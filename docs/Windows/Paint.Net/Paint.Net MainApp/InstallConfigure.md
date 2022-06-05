# Installation and Configuration Notes for Paint.Net (Main App)

By default the app will install into the user programs folder `paint.net` by default.

## Project Evergreen
Project Evergreen AppTracker provides information and sources for installers for this app https://stealthpuppy.com/apptracker/#paintdotnetofflineinstaller 


## EXE based installer

The main exe installer supports silent installation and other options. 
* For example, use '/auto CHECKFORUPDATES=0 JPGPNGBMPEDITOR=1 TGAEDITOR=1 DESKTOPSHORTCUT=0'.


## SilentInstallHQ
Silent Install HQ provides information on the silent install of this app here: https://silentinstallhq.com/?s=paint.net.

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* Plugins are dlls that may be copied into a `Effects` or `FileTypes` folder under the main install, dependent on the type of plugin.
* The product does have an autoupdater.  There is an installation option to disable it.  


## Installed Components worth noting

* There is one shortcut.
* There are FTAs, both new and updates to existing.
* There is a Shell Extension (image handler).
* There are FTA  shell integraion menus.
* There is an App Paths registration.
* The app does not add files to AppData\Local or Roaming.