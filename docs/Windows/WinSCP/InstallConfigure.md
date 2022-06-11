# Installation and Configuration Notes for WinSCP
By default the app will install under the apprpriate Program Files (x86) folder.

## Project Evergreen
Project Evergreen AppTracker provides information and sources for installers for this app here: https://stealthpuppy.com/apptracker/#winSCP .

## SilentInstallHQ
Silent installation information is available from SilentInstallHQ for this app from this link: https://silentinstallhq.com/?s=winSCP .

## EXE based installer

Supports silent installation. The installer is built on an older InstallShield framework, supporting an iss file style configuration.  This means that you can run the installer to save an .iss configuration file from the settings that you choose and use it for subsequent installation. For example '"/ALLUSERS /SP- /SILENT /VERYSILENT /SUPRESSMSGBOXES /LOADINF=$($executingScriptDirectory)\Settings.iss"'.  Use '/?' for more options.


## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* The product has an autoupdater built in.  This is disabled via registry.
* It is common to remove the desktop shortcut.
* It is possible to preconfigure a site in the registry, however the password should not be saved.

## Installed Components worth noting

* The application installs with one shortcut in the start menu and another on the desktop. 
* The application has a Copyhook Shell extension for the special FTA 'Directory'. 
* The application has numerous protocol handlers.
* The application has no services.