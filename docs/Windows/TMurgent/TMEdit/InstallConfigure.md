# Installation and Configuration Notes for TMEdit

The application is delivered in a setup exe installer. By default it installs to the Progam Files area.  


## Project Evergreen
Project Evergreen AppTracker does not provide information and sources for installers for this app when last checked.


## EXE based installer

Installer supports a silent installation. It has an embedded MSI, so use:
* Use "/exenoui /qn"

## SilentInstallHQ
Silent Install HQ provides no information on the silent install of this app.

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* Registration must be done by the end user.
* 

## Installed Components worth noting

* 1 Shortcut
* 1 FTA (.appv) with Shell Integration Command.
* No Shell Extensions, Protocol Handlers, or Services.
* The app installer does not install anything in the user's AppData\Local or Roaming folders.
* The app has a notification for updates that is not configurable.  It does not perform the update but allows the end-user to download an updated installer into the browser downloads folder.  The update notice isn't prominent.
