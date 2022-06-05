# Installation and Configuration Notes for Filezilla

By default the app will install under a `Filezilla` folder in the Program Files folder.

## Project Evergreen
Project Evergreen AppTracker provides information and sources for installers for this app https://stealthpuppy.com/apptracker/#filezilla 


## EXE based installer

The main exe installer supports passive installation:
* Use  '/S /D=C:\Program Files\Filezilla' for silent installation.
* Remove unnecessary shortcut to `Uninstall`.



## SilentInstallHQ
Silent Install HQ provides this information on the silent install of this app: https://silentinstallhq.com/?s=Filezilla 

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* The application uses an xml file for the configuration. This file should be placed as the User's AppData\Local\FileZilla\FileZilla.xml 
* The product does have an autoupdater. Set `Update Check` to 0 in the configuration xml file.
* Other customizations were not tested.

## Installed Components worth noting

* The application install uses the AppData\Local folder. 
* Two shortcuts are placed, but normally we remove the Uninstall shortcut.
* There is an FTA on DIRECTORY for a CopyHook shell extension.  This extension is important functionality to how users typically use the product.
