# Installation and Configuration Notes for Firefox

By default the app will install under a `Firefox` folder in the Program Files folder.

The software has an updater that is implemented as a windows service.  Disable the service to disable updates.

## Project Evergreen
Project Evergreen AppTracker provides information and sources for installers for this app https://stealthpuppy.com/apptracker/#mozillafirefox 


## EXE based installer

The main exe installer supports silent installation:
* Use  '/S /DesktopShortcut=false /MaintenanceService=false /RemoveDistributionDir=true /RegisterDefaultAgent=false' for silent installation.
* NOTE: Recent versions of the exe installer launch firefox after install.  I have not found a switch to disable it, so you should go with the msi installer.

## MSI based installer

The MSI installer supports normal switches.
* For example, use '/passive DESKTOP_SHORTCUT=false INSTALL_MAINTENANCE_SERVICE=false'.



## SilentInstallHQ

Silent Install HQ provides this information on the silent install of this app: https://silentinstallhq.com/?s=Firefox 

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* The application uses the registry for configuration, however a `policies.json` file may be copied into the `distribution` subdirectory of the install location (C:\program files (x86)\Mozilla Firefox\distribution).  It also may be controlled externally via group policy.  More information from vendor https://support.mozilla.org/en-US/kb/customizing-firefox-using-policies.json  
* Disable or remove the Mozilla maintenance service to get rid of auto-updates.

## Installed Components worth noting
 
* Two identical shortcuts are placed, one for all user's and one for the current user.
* There is an FTA on .shmtl  (Shell integration not extension).
* There is one URL handler (purpose unknown but possibly related to updates).
