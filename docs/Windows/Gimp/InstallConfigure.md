# Installation and Configuration Notes for Gimp

By default the app will install under a `Gimp 2` folder in the Program Files folder.

This application has many available plugins built-in.

## Project Evergreen
Project Evergreen AppTracker provides information and sources for installers for this app https://stealthpuppy.com/apptracker/#gimp 


## SilentInstallHQ
Silent Install HQ provides this information on the silent install of this app: https://silentinstallhq.com/?s=gimp 


## EXE based installer

The main exe installer supports passive installation:
* Use  '/VERYSILENT /SUPPRESSMSGBOXES /NORESTART /SP-' for silent installation.



## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* As the application is developed to be cross-platform, it has little in the way of windows integrations and end-user customizations.  
* There are a number of xml, ini, and cfg files in the installation folders, and there are also files without a file extension that are text based configuration files, however it is not clear if any actually require being opened for write purposes.  Changes made by the runtime program appear to automatically be routed to the user's AppData\Roaming folder.
* The only registry use is for the FTAs, whch there are a lot of (67 at one count).  These are all shell integration commands and there are no shell extensions.
* There is an updater that can be turned off in the Edit->Preferences dialog (System screen). This will write to the gimprc file in the AppData/Roaming area.  The line that is transformed is:

| From | To |
|----|----|
| (check-updates yes) | (check-updates no) |

The value may also be changed in the same named file under `Program Files\Gimp 2` as long as the user does not already have a copy under AppData/Roaming.

The end-user can still re-enable this in the Preferences dialog.

## Installed Components worth noting

* The application install does not use the AppData\Local or Roaming folders. 
* One shortcut is placed.
