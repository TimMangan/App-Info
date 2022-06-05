# Installation and Configuration Notes for Project Libre

By default the app will install under a `AceBit` folder in the Program Files folder.

## Project Evergreen
Project Evergreen AppTracker provides information and sources for installers for this app https://stealthpuppy.com/apptracker/#projectlibre 


## EXE based installer

The EXE installer may be silently installed:
 * For example: '/SP- /SILENT /SURPRESSMSGBOXES /ACCEPTEULA=1'

The application may be configured via registry.  The app uses HKCU\Software\JavaSoft.  Here is an example .reg file

```reg
Windows Registry Editor Version 5.00

[HKEY_CURRENT_USER\SOFTWARE\JavaSoft\Prefs\com\projectlibre1]

[HKEY_CURRENT_USER\SOFTWARE\JavaSoft\Prefs\com\projectlibre1\dialog]
"license/Validation/Date"="1627510474378.567"
"validated/License"="true"
"user/Email"=""
"tip/Number"="3"
"/Show/Tip/On/Startup"="false"

[HKEY_CURRENT_USER\SOFTWARE\JavaSoft\Prefs\com\projectlibre1\main]
"projectlibre/Run/Number"="3"
"projectlibrefirst/Run"="1627510469144"

[HKEY_CURRENT_USER\SOFTWARE\JavaSoft\Prefs\com\projectlibre1\preference]

[HKEY_CURRENT_USER\SOFTWARE\JavaSoft\Prefs\com\projectlibre1\util]
"/Java/Version"="1.8.0_172"
"/P/O/D/Version"="1.9.3"
```

## SilentInstallHQ

Silent Install HQ provides this information on the silent install of this app: https://silentinstallhq.com/?s=Project+Libre.

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* Disabling Eula and other first run dialogs shown in the reg file above.

## Installed Components worth noting
 
* The application installs into program files.
* There is one shortcut installed.
* The app does not install, or require, any version of Java.
