# Installation and Configuration Notes for Sigil

By default the app will install into the user programs folder by default.


## EXE based installer


The main exe installer supports passive and silent installation:
* For example, use '/ALLUSERS /NORESTART /SP- /VERYSILENT /SUPPRESSMSGBOXES /COMPONENTS="*afiles,vcruntimeadmin"' .

The installer adds two shortcuts to the start menu.  One is an uninstaller (unins000) which may be removed.

## SilentInstallHQ
Silent Install HQ provides no information on the silent install of this app.

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* The product does not have an autoupdater.
* Other customizations were not tested.

## Installed Components worth noting

* The application install has configuration files under Program Files. It is unclear as to what might trigger these being updated by the end-user. 
* It does not install any files to AppData local or remote by default.
* Is uses a file under %localappdata%\sigil-ebook\sigil for user preferences.
