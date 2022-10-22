# Installation and Configuration Notes for TeamViewer

By default the app will install into the user programs folder by default.

## Project Evergreen
Project Evergreen AppTracker provides information and sources for installers for this app https://stealthpuppy.com/apptracker/#teamviewer 

## EXE based installer


The main exe installer supports passive installation:
* Use '/S' for silent installation.

The installer adds a shortcut to the start menu and to the desktop.  Often removing the desktop shortcut is desired.

Preconfiguraton to defeat the updater is available in the registry.  See sample reg file below:

```reg
Windows Registry Editor Version 5.00

[HKEY_LOCAL_MACHINE\SOFTWARE\TeamViewer]
"UpdateChannel"=dword:00000001
"AutoUpdateMode"=dword:00000003
"UpdateCheckInterval"=dword:00000002
```

## SilentInstallHQ
Silent Install HQ provides this information on the silent install of this app: https://silentinstallhq.com/?s=teamviewer  

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* The product does have an autoupdater.
* Installer placed a "TeamViewer" shortcut on the desktop.
* Other customizations were not tested.

## Installed Components worth noting

* 
