# Installation and Configuration Notes for 7-zip
By default the app will install into a `7-Zip` folder under the apprpriate Program Files folder.

## Project Evergreen
Project Evergreen AppTracker provides information and sources for installers for this app https://stealthpuppy.com/apptracker/#7zip 

## Exe based installer

Silent installation is possible:  

* "/S" (capitalized) for silent installation. 

## MSI based installer

Normal MSI parameters are available for quick/passive/silent installation, and:

* INSTALLDIR is supported.
* ALLUSERS is supported.

## SilentInstallHQ
Silent Install HQ provides information on the silent install of this app https://silentinstallhq.com/?s=7-zip



## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* The product does not currently have an autoupdater built in.
* Registry based configuration available under the key `[HKEY_CURRENT_USER\SOFTWARE\7-Zip\FM]`.  None of these items appear critical.

## Installed Components worth noting

* The application installs with two shortcuts, one for the program and another for the chm-based help file.  The help is alao available from in the program so the latter shortcut may be removed.
* The application adds/updates a lot of file type associations for compressed file formats, and consideration should be made if this app should become the default for these file types.  Most of these FTAs are for Shell Integration (verb/command) access.
* The application has several shell extensions:
* * 2 Context Menu handlers (one for all file types and another for Directories).
* * A Drag&Drop handler.
* The application includes an App Paths registration for both search (execution alias) and dll loading.
* Although there is an uninstall.exe file in the installation folder, there is no shortcut to it.
* The installed app does not use AppData local or roaming folders, however the runtime will use the temp folder for temporary storage.