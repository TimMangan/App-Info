# Installation and Configuration Notes for Opera

By default the app will install under a `Opera` folder in the Program Files folder.


## EXE based installer

The EXE installer supports a lot of switches.  For example, use 
* '/SILENT /norestart /allusers=0 /launchopera=0 /desktopshortcut=0 /setdefaultbrowser=0 /pintotaskbar=0 /enable-stats=0  --with-feature:installer-use-minimal-package'.


## SilentInstallHQ

Silent Install HQ provides this information on the silent install of this app: https://silentinstallhq.com/?s=Opera

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* The application uses the files for configuration. 
* The command line options shown in the 'EXE based installer' section above takes care of a bunch of things to start.
* Optionally create a file called `preferences` that contains preconfigured preferences (such as to enable ad-blocker) and copy it to the user's `AppData\Roaming\Opera Software\Opera Stable` folder.
* Modify the shortcut to Opera to add `--disable-update` as command line argument.

## Installed Components worth noting
 
* No files in AppData/Local or Roaming by the installer, however configuration information is stored in both locations.
* There is an updater, enabled by default.  This may be turned off through a file in the user's appdata\local folder. Unfortunately, the software generates a system hash for the path to this file so automated packaging to turn this off is not pratical except by end-user.  But this is the same as with a native install.
* No FTAs or Shell Extensions.
* Lots of ActiveX.
