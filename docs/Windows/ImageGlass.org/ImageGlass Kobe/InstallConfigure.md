# Installation and Configuration Notes for ImageGlass Kobe

By default the app will install under a `ImageGlass` folder in the Program Files folder.


## MSI based installer

The main exe installer supports passive installation:
* Use  '/q RUNAPPLICATION="0" IAGREE="Yes"' for silent installation. These options keep the app from launching after install, and take care of the EULA.
* Remove the desktop shortcut.
* Optionally copy pre-pared igconfig.xml and igstartup.profile file to the AppData/Roaming/ImageGlass folder.


## SilentInstallHQ
Silent Install HQ provides no information on the silent install of this app at this time.

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* The igconfig.xml file is the general configuration file. It contains a setting for the AutoUpdater, which is enabled by default.  Set as `<Item key="AutoUpdate" value="0" />` to disable.


## Installed Components worth noting

* The application itself does not install uses the AppData\Roaming or Local folders. 
* There are no FTAs or Shell Extensions by default.  FTAs may be enabled by the end-user.
