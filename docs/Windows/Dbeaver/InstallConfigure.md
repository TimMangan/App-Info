# Installation and Configuration Notes for Dbeaver

By default the exe installer for this app will install into folder `DBeaver` under  `Program Files`.  It includes a copy of it's own Java JRE.

## Project Evergreen
Project Evergreen AppTracker provides information and sources for installers for this app at this link: https://stealthpuppy.com/apptracker/#dbeaver 

## Vendor Silent Install Documentation
The project site documents the installation options on this page: https://github.com/dbeaver/dbeaver/wiki/Windows-Silent-Install


## SilentInstallHQ
Silent Install HQ provides information on the silent install of this app here: https://silentinstallhq.com/?s=dbeaver

## EXE based installer
The EXE installer uses '/S', but you must then also specify all or current users. Note that these are case sensitive:
*   /S /allusers
*   /S /currentuser

The /currentuser option will only install into the user's appdata/local folder.  Using the /allusers option allows you to add /D "C:\Program Files\DBeaver" to the END of the command line.  /? says you can't have quotes, but it works.




## Typical Configuration Items 
WIP - want to shut off updater. The docs hint that this can be disabled, have not found how. 
Typically want to remove start menu uninstall shortcut.

## Installed Components worth noting

* There is one shortcut for the app.  It has an argument for the language (eg '-nl en') but product defaults to the os locale when not present.
* There is an optional argument, not present, '-nosplash' that can be added to the shortcut
* Initial launch wants to set up firewall rule, then asks if you want to set up a sample database, then to select a database to start with.


## WIP
* The app installs some configuration into the user profile under `C:\Users\xxx\.elipse`. 
* * The file  `C:\Users\xxx\.elipse\.settings\org.eclipse.ui.ide.prefs` looks interesting.
* The app uses AppData\Roaming\DBeaverData folder for "workspace" and "driver" storage.  It might be possible to run app and connect to a database and keep that in the package. Credentials storage?

### WIP Updaters
You can disable updaters in GUI using the Menu: `Window-->Preferences\General\Install/Update\Available Software Sites`.

This seems to store in two text based files:
    `C:\Users\admin\.eclipse\org.jkiss.dbeaver.product_22.1.0_1535670467_win32_win32_x86_64\p2\org.eclipse.equinox.p2.artifact.repository.prefs`
    `C:\Users\admin\.eclipse\org.jkiss.dbeaver.product_22.1.0_1535670467_win32_win32_x86_64\p2\org.eclipse.equinox.p2.engine\profileRegistry\DefaultProfile.profile\.data\.settings\org.eclipse.equinox.p2.metadata.repository.prefs`

There are also ini and other files in the PF area.  This one is interesting:
    `C:\Program Files\DBeaver\configuration\org.eclipse.update\platform.xml`
