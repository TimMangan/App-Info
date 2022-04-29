# Installation and Configuration Notes for Fiddler (Classic)

By default the app will install into the user programs folder by default.


## EXE based installer


The main exe installer supports passive installation:
* Use '/S /D=C:\Program Files\Fiddler' for silent installation.

The installer adds a shortcut to the start menu and to the desktop.

## SilentInstallHQ
Silent Install HQ provides this information on the silent install of this app: https://silentinstallhq.com/?s=fiddler 

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* The product does not have an autoupdater.
* Other customizations were not tested.

## Installed Components worth noting

* The application install uses both AppData\Local folder.  It wants to install to the user's program folder so specifying a normal folder in the installer is suggested.
* Older versions of the app included a plugin to Internet Explorer, but this has been removed in v5.
The app has a one-time check that prompts that this version is quite old, but have not determined how to disable it yet.
* There are two shortcuts, and a FTA (.saz).
* The app installation relies on a change to the PATH envorinmental variable to find dlls.
* General configuration of the app may be done via the registry in an incorrect location:(HKCU\Software\Microsoft\Fiddler2)