# Installation and Configuration Notes for WinMerge
By default the app will install under the apprpriate Program Files folder.

## Project Evergreen
Project Evergreen AppTracker provides information and sources for installers for this app here: https://stealthpuppy.com/apptracker/#winmerge .

## SilentInstallHQ
Silent installation information is available from SilentInstallHQ for this app from this link: https://silentinstallhq.com/?s=winmerge .

## ZIP based installer

Is available, but not tested.

## EXE based installer

Supports silent installation, for example '/SP- /VERYSILENT /SUPRESSMSGBOXES'.  Use '/?' for more options.

The x64 version has a per-system or per-user installer.  The per-system installer was tested.


## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* The User Guide shortcut should be renamed to WinMerge User Guide so that the icons stay together in the Windows 10 menu. Or removed.
* The product does not currently have an autoupdater built in.
* The product does not have any configuration settings.

## Installed Components worth noting

* The application installs with two shortcuts. One is a link to the User's Guide file.
* The application has no Protocol handlers or services.
* The application has several FTA Shell Extensions, including Context Menu, and Drag-and-drop handlers. These are all implemented in the same COM Shell extension. In addition to a new .WinMerge FTA, the special "*", "Directory", and "Drive" FTAs are updated.
* The application has no Protocol handlers or services.
* The application adds no files to the AppData Local or Roaming folders (when the system wide installer is used).