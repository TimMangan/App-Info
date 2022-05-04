# Installation and Configuration Notes for OBS Studio

By default the app will install under a `obs-studio` folder in the Program Files folder.




## EXE based installer

The EXE installer supports silent installation, for example:
* '/S' for silent (captial S)
* '/S /D=C:\folder' to also set the installation folder.


## SilentInstallHQ

Silent Install HQ provides this information on the silent install of this app: https://silentinstallhq.com/?s=OBS 

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* The application adds a second shortcut to the desktop (remove if not desired).
* The application adds an `Uninstall.lnk` shortcut to the start menus (remove if not desired). 
* The application uses file-based configuration `global.ini` placed in a `obs-studio` subfolder of the user's AppData\Roaming.
* * It has an autoupdate setting to disable
* * It has as well as a first run setting you might disable.
* * It has a tray icon you might or might not want to disable.

## Installed Components worth noting
 
* There are no FTAs or Shell Extensions, or other integrations.
* The installer does not add needed files to the AppData\Local folders, however there may be DirectX3D lock files present that should probably be removed when repackaging.
* The installer does not add files to the AppData\Roaming folder (although the 'typical' configuration above does).
