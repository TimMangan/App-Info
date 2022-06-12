# Installation and Configuration Notes for Trimble SketchupViewer

The application is delivered in a setup exe installer. By default it installs to the Progam Files area.  


## Project Evergreen
Project Evergreen AppTracker does not provide information and sources for installers for this app when last checked.


## EXE based installer

Installer supports a silent or passive installation:
* Use '/silent' or '/passive'

## SilentInstallHQ
Silent Install HQ provides no information on the silent install of this app.

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* The installer puts an extra shortcut on the desktop 'SketchUp Viewer 2021.lnk' and a log file 'ViewerInstallShield.log'.  These are typically removed.
* Other configuration options were not tested, however there is a EULA that might be disabled.

## Installed Components worth noting

* The setup exe uses InstallShield for the framework.  It has an embedded msi and installs a version of the VC Runtime (vc140).
* 1 FTA (.skp) with Shell Integration Command and ShellNew entry.
* No Shell Extensions, Protocol Handlers, or Services.
* The app installer does not install anything in the user's AppData\Local or Roaming folders.
