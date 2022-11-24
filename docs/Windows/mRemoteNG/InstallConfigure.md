# Installation and Configuration Notes for mRemoteNG

By default the app will install under a `mRemoteNG` folder in the Program Files (x86) folder.

## Project Evergreen
Project Evergreen AppTracker provides information and sources for installers for this app https://stealthpuppy.com/apptracker/#mremoteng


## ZIP based installer

Unpack to a folder and create a shortcut.

## MSI based installer

The MSI installer supports normal switches.
* For example, use '/passive' or '/qn'.


## SilentInstallHQ

Silent Install HQ provides this information on the silent install of this app: https://silentinstallhq.com/?s=mremote

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* The application uses the registry for configuration, however these settings are set by the installer and typically not changed.
* The application has a mRemoteNG.exe.Config file which may be altered for the preconfiguration.  This is the only way to disable the update feature. 
* Shortcuts to 'Credits.lnk', 'License.lnk', and 'Readme.lnk', may be removed. If left on Windows 10/11 editing the names to start with mRemoteNG is recommended.

## Installed Components worth noting
 
* No files in AppData/Local or Roaming by the installer, however configuration information is stored in both locations.
* There is an updater, enabled by default.  This may be turned off through a file in the program folder (mRemoteNG.exe.Config). You can overwrite this file after installation to pre-configure.
* No FTAs or Shell Extensions.
* Lots of ActiveX.
