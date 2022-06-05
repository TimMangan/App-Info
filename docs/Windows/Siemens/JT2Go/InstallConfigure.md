# Installation and Configuration Notes for JT2Go

By default the app will install into the user programs folder by default.

## Project Evergreen
Project Evergreen AppTracker does not provide information and sources for installers for this app when last checked.


## EXE based installer


The main exe installer supports passive and silent installation:
* Copy the JT2GoSetup.exe file into a new folder created in the temp folder.
* Copy an edited version of the CustomInstall.cmd file to the same folder (script shown below).
* Create a folder %localAppData5\Siemens\myConfig
* cd to the temp folder.
* Run the CustomInstall.cmd file (elevated.)
* Disable the EULA via registry change (script shown below).

Here is a sample cmd file:

```cmd
f
rem --------------------------------------------------------------------
rem
rem This script provides a template for customizing and launching the
rem JT2Go 13.3 installer.  Controlling the installer in this manner will:
rem
rem     * allow for preselection of features to be installed
rem     * prefill required fields (e.g. licensing options)
rem     * ease deployment to a large number of users.
rem
rem To use this script, simply uncomment and fill in the proper options
rem below, and choose the proper options for the install, or feel free
rem to otherwise modify it to fit your situation.
rem
rem For some Windows Installer options, there are more possible values than
rem are listed here.  For the complete Windows Installer command line reference, see
rem http://msdn.microsoft.com/library/default.asp?url=/library/en-us/msi/setup/command_line_options.asp
rem
rem --------------------------------------------------------------------

setlocal

set EXEFILE=JT2GoSetup.exe
set OPTIONS=

rem --------------------------------------------------------------------
rem Silent mode. OPT1 is for the .exe wrapper, OPT2 is standard Windows
rem Installer silent mode option.  Both must be set.
rem --------------------------------------------------------------------
rem set SILENTOPT1=/S &set SILENTOPT2=/qb
set SILENTOPT1=/S &set SILENTOPT2=/qb

rem --------------------------------------------------------------------
rem Installer logging
rem --------------------------------------------------------------------
rem set OPTIONS=%OPTIONS% -l*v C:\temp\JT2GoIns.log
set OPTIONS=%OPTIONS% -l*v C:\Users\Public\Documents\SequencedPackage\JT2GoIns.log

rem --------------------------------------------------------------------
rem set the language in which to run the installer
rem --------------------------------------------------------------------
set ILANG=/L1033 &rem English
rem set ILANG=/L1036 &rem French (Standard)
rem set ILANG=/L1031 &rem German
rem set ILANG=/L1040 &rem Italian (Standard)
rem set ILANG=/L1034 &rem Spanish - Traditional Sort
rem set ILANG=/L1029 &rem Czech
rem set ILANG=/L1045 &rem Polish
rem set ILANG=/L1046 &rem Portuguese (Brazil)
rem set ILANG=/L1049 &rem Russian
rem set ILANG=/L1041 &rem Japanese
rem set ILANG=/L1042 &rem Korean
rem set ILANG=/L1052 &rem Chinese (Simplified/PRC)
rem set ILANG=/L1028 &rem Chinese (Traditional/Taiwan)


rem --------------------------------------------------------------------
rem Set the Install-to directory
rem --------------------------------------------------------------------
rem set OPTIONS=%OPTIONS% INSTALLTO=\"C:\Program Files\Siemens\JT2Go\"
set OPTIONS=%OPTIONS% INSTALLTO=\"C:\Program Files\Siemens\JT2Go\"

rem --------------------------------------------------------------------
rem set foreign language localizations to be installed (optional)
rem --------------------------------------------------------------------
rem set OPTIONS=%OPTIONS% INSTALL_SPANISH=1
rem set OPTIONS=%OPTIONS% INSTALL_GERMAN=1
rem set OPTIONS=%OPTIONS% INSTALL_FRENCH=1
rem set OPTIONS=%OPTIONS% INSTALL_ITALIAN=1
rem set OPTIONS=%OPTIONS% INSTALL_CZECH=1
rem set OPTIONS=%OPTIONS% INSTALL_PORTUGUESE=1
rem set OPTIONS=%OPTIONS% INSTALL_POLISH=1
rem set OPTIONS=%OPTIONS% INSTALL_JAPANESE=1
rem set OPTIONS=%OPTIONS% INSTALL_KOREAN=1
rem set OPTIONS=%OPTIONS% INSTALL_SCHINESE=1
rem set OPTIONS=%OPTIONS% INSTALL_TCHINESE=1
rem set OPTIONS=%OPTIONS% INSTALL_RUSSIAN=1


rem --------------------------------------------------------------------
rem Install a Desktop Shortcut. 1=yes, 0=no. Default=1
rem --------------------------------------------------------------------
rem set OPTIONS=%OPTIONS% DT_SHORTCUT=0
set OPTIONS=%OPTIONS% DT_SHORTCUT=0

rem --------------------------------------------------------------------
rem Disable internet connection for JT2Go session. 1=yes, 0=no. Default=0
rem --------------------------------------------------------------------
rem set OPTIONS=%OPTIONS% DISABLE_INTERNET=1
set OPTIONS=%OPTIONS% DISABLE_INTERNET=0

rem --------------------------------------------------------------------
rem Disable automatic updates. 1=yes, 0=no. Default=0
rem --------------------------------------------------------------------
rem set OPTIONS=%OPTIONS% DISABLE_UPDATES=1
set OPTIONS=%OPTIONS% DISABLE_UPDATES=1

rem --------------------------------------------------------------------
rem set initial behavior for the Teamcenter Visualization Product Excellence Program
rem Valid values are:
rem   0: UI enabled, checkbox off (Product Excellence Program disabled, end user can change thru UI)
rem   1: UI disabled, checkbox off (Product Excellence Program disabled, end user cannot change)
rem   2: UI enabled, checkbox on (Product Excellence Program enabled, end user can change thru UI)
rem   3: UI disabled, checkbox on (Product Excellence Program enabled, end user cannot change)
rem --------------------------------------------------------------------
rem set OPTIONS=%OPTIONS% JT2GO_PEP_INIT=1
set OPTIONS=%OPTIONS% JT2GO_PEP_INIT=1

rem --------------------------------------------------------------------
rem Location of configuration file (optional)
rem Either use a UNC path to the version specific CONFIG_JT2Go file, or copy it locally.
rem --------------------------------------------------------------------
rem set OPTIONS=%OPTIONS% CONFIG="C:\temp\myConfig"
set OPTIONS=%OPTIONS% CONFIG="%LocalAppData%\Siemens\myConfig"

rem --------------------------------------------------------------------
rem Enable installer-time import of default registry settings. 1=yes, 0=no. Default=0
rem   If not installed at install time, launching JT2Go for the first 
rem   time will import them anyway using regedit.
rem --------------------------------------------------------------------
rem set OPTIONS=%OPTIONS% IMPORTDEFAULTREG=1
set OPTIONS=%OPTIONS% IMPORTDEFAULTREG=1

rem launch the installer
START /WAIT %EXEFILE% %ILANG% %SILENTOPT1% /v"%SILENTOPT2% %OPTIONS%"


endlocal
```

```ps1
# Stop Eula in all environments for installed version (good until version 20)
    $keyname = 'Software\Siemens\JT2Go'
    New-PassiveRegistryKeyIfNotPresent -Hive "HKCU" -Key $keyname
    $keys = Get-item "HKCU:\$($keyname)"
    foreach ($ppkey in $keys)
    {
        if ($ppkey.Name.Contains('1'))
        {
            $pkeyname = "Software\Siemens\JT2Go\$($ppkey)\JT2Go"
            New-PassiveRegistryKeyIfNotPresent -Hive "HKCU" -Key $pkeyname
            $pkey  = Get-item "HKCU:\$($pkeyname)"
            $skeys = $pkey.GetSubKeyNames()
            foreach ($skey in $skeys)
            {
                New-PassiveRegistryKeyIfNotPresent -Hive "HKCU" -Key "$($pkeyname)\$($skey)\CurrentProfile"
                set-itemproperty -Path "HKCU:\$($pkeyname)\$($skey)\CurrentProfile" -Name 'Agreement' -Value 1   
            }
        }
    }
```

The installer adds one shortcut to the start menu. 

## SilentInstallHQ
Silent Install HQ provides no information on the silent install of this app.

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* See sample setup cmd and ps1 files above.


## Installed Components worth noting

* The product does have an autoupdater, but may be disabled via the cmd script to install.  I
* No FTA, shell extensions, or services.
* One Protocol handler (JTCmd) that uses a ProgID.
