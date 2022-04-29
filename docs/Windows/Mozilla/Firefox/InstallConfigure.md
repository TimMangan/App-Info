# Installation and Configuration Notes for Firefox

By default the app will install under a `Firefox` folder in the Program Files folder.

The software has an updater that is implemented as a windows service.  Disable the service to disable updates.

## EXE based installer

The main exe installer supports silent installation:
* Use  '/S /DesktopShortcut=false /MaintenanceService=false /RemoveDistributionDir=true /RegisterDefaultAgent=false' for silent installation.

## MSI based installer

The MSI installer supports normal switches.
* For example, use '/passive DESKTOP_SHORTCUT=false INSTALL_MAINTENANCE_SERVICE=false'.



## SilentInstallHQ

Silent Install HQ provides this information on the silent install of this app: https://silentinstallhq.com/?s=Firefox 

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* The application uses the registry for configuration. 
* Disable or remove the Mozilla maintenance service to get rid of auto-updates.

## Installed Components worth noting
 
* Two identical shortcuts are placed, one for all user's and one for the current user.
* There is an FTA on .shmtl  (Shell integration not extension).
* There is one URL handler (purpose unknown but possibly related to updates).
