# Installation and Configuration Notes for Everything
By default the app will install under the apprpriate Program Files folder.

## Project Evergreen
Project Evergreen AppTracker provides information and sources for installers for this app here: https://stealthpuppy.com/apptracker/#voidtoolsEverything .

## SilentInstallHQ
Silent installation information is available from SilentInstallHQ for this app from this link: https://silentinstallhq.com/?s=everything .

## ZIP based installer

Is available, but not tested.  They call this the portable version in documentation.  You'd unzip and then silently install using information  on the forum site post: https://www.voidtools.com/forum/viewtopic.php?f=5&t=5673 

For example `-install "C:\Program Files\Everything" -install-options "-app-data -install-service -install-efu-association -install-run-on-system-startup -install-start-menu-shortcuts -install-language 1033" `. 

The installer does not allow for setting of what they consider to be user options.  To silently set those, the program may be run with command line arguments.  For example
`"C:\Program Files\Everything\Everything.exe" -disable-update-notification -uninstall-quick-launch-shortcut`

## EXE based installer

Supports silent installation, using information on the forum site post: https://www.voidtools.com/forum/viewtopic.php?f=5&t=5673 

For example `/S /D="C:\Program Files\Everything" -install-options "-app-data -install-service -install-start-menu-shortcuts -install-efu-association -install-url-protocol -install-language 1033" `. 

The installer does not allow for setting of what they consider to be user options.  To silently set those, the program may be run with command line arguments.  For example
`"C:\Program Files\Everything\Everything.exe" -disable-update-notification -uninstall-quick-launch-shortcut`



## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* There are a lot of options on how this product is configured and used in the enterprise, including the possibility of organizing the data through an external server.  Beyond the simple things covered above, other options will be customer specific.
* The app adds a Run key to start the app up in the background in order to speed up getting results when the user launches the app.  This may not be wanted.

## Installed Components worth noting

* The application install may be limited to one shortcut.
* The application has an optional Protocol handler and optional service.  The service seems to avoid the need for elevation of the app so you probably want that in an enterprise environment.
* The application uses the AppData Roaming folder for storage by default.
