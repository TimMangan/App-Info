# Installation and Configuration Notes for Postman

By default the app will install under a `AceBit` folder in the Program Files folder.

## Project Evergreen
Project Evergreen AppTracker provides information and sources for installers for this app https://stealthpuppy.com/apptracker/#postman 

## EXE based installer

The EXE installer supports is unpackager that then relaunches itself.  This can be automated with the following:

```ps1
    WRITE-HOST "Note: Installer relaunches itself, so pause and wait for it by name"
    Start-Process "$($executingScriptDirectory)\Postman-win64-9.8.2-Setup.exe" -ArgumentList '-s' -NoNewWindow -Wait
    Start-Sleep 10
    Wait-Process 'Postman-win64-9.8.2-Setup' -Timeout 600
```

## SilentInstallHQ

Silent Install HQ provides this information on the silent install of this app: https://silentinstallhq.com/?s=postman.

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* None identified

## Installed Components worth noting
 
* The application installs into AppData/Local.
* There is one shortcut installed.
* There are no FTA, Shell Extensions, Protocol Handlers, Services.
