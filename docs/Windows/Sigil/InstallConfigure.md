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

* The product does have an autoupdater.  It is hard coded to look for updates at launch every 6 hours.  It stores a timestamp, along with the current version found, in an ini file (%localappdata%\sigil-ebook\sigil\sigil.ini) in a section similar to shown below:

```ini
[updatechecker]
last_check_time=@DateTime(\0\0\0\x10\0\0\0\0\0\0%\x88U\x2\x14\xe2\x19\0)
last_online_version=1.9.10
```

It may be possibly to package up a pre-deployed version of this file by running the app once and then editing the last_check_time to a value well into the future.  It should represent the current date time at the time of the last check.  You can run a test install to create this file (use edit->preferences to set anything else as well). Copy this file (you don't need the others) and edit the last_check_time.  I would replace the portion "\0%" with "\xff%". Copy this file into the folder location as part of a post install script.  I haven't decifered the format, but I think this sets a date way into the future.

PS: Altering the last_online_version value doesn't help once a newer version becomes available.  It will be reset to the current latest version each time the app starts up.



* Other customizations were not tested.

## Installed Components worth noting

* The application install has configuration files under Program Files. It is unclear as to what might trigger these being updated by the end-user. 
* It does not install any files to AppData local or remote by default.
* Is uses a file under %localappdata%\sigil-ebook\sigil for user preferences.
