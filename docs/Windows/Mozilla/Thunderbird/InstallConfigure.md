# Installation and Configuration Notes for Thunderbird

By default the app will install under a `Mozilla Thunderbird` folder in the Program Files folder.

The software has an updater that is implemented as a windows service.  Disable the service to disable updates.

## Project Evergreen
Project Evergreen AppTracker provides information and sources for installers for this app https://stealthpuppy.com/apptracker/#mozillathunderbird 




## MSI based installer

The MSI installer supports normal switches.
* For example, use '/passive DESKTOP_SHORTCUT=false INSTALL_MAINTENANCE_SERVICE=false' to get rid of the desktop shortcut and stop the updater service.


## SilentInstallHQ

Silent Install HQ provides this information on the silent install of this app:https://silentinstallhq.com/?s=Thunderbird

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* The application uses the registry for configuration. 
* Disable or remove the Mozilla maintenance service to get rid of auto-updates.  
* Remove desktop shortcut if not desired.

It is possible to add more control by dropping a policies.json file into the Program Files(x86)\Mozilla\Thunderbird\distribution folder.  
There is a setting to disable updates, but you can control extensions, forcing some to be installed and preventing others.  The json below disables the updates; see Thunderbird website for details on the extensions.

```json
{
    "policies": {
        "DisableAppUpdates": true
    }
}
```

## Installed Components worth noting
 
* Two identical shortcuts are placed, one for all user's and one for the current user.
* There are no FTAs or Shell Extensions
* There is a Software Client registration for email.
* There are internal COM servers for MAPI  and maybe accessibility handler.
* The installer does not add files to the AppData\Local or Roaming folders.
