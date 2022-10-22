# Installation and Configuration Notes for VlcPlayer
By default the app will install under the apprpriate Program Files folder.

## Project Evergreen
Project Evergreen AppTracker provides information and sources for installers for this app at https://stealthpuppy.com/apptracker/#videolanvlcplayer .

## Silent Install
SilentInstallHQ provides information on this app at https://silentinstallhq.com/?s=VLC .

## EXE based installer

Supports silent installation, for example '/S'. 

## MSI based installer

Supports silent ('/qn') or passive ('/passive') options.

## Typical Configuration Items 

The app stores configuration only after first run.  This includes a setting for the autoupdate.  We can pre-configure this and copy to the user's appdata\roaming\vlc folder.  There will be three files to be copied if you want to preconfigure this.


## Installed Components worth noting

* The application installs with a lot of shortcuts to the start menu and one to the destop.    Typically,only one shortcut is desired for this app.
* Removal of uninstall.exe is possible.
* The application has a lot of FTA, each with multiple command verbs.
* The application has no Shell Extensions, or Protocol handlers.
* The application has no services.
