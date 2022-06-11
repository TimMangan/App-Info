# App-Info Install/Configure for VSCode

The application is delivered in a setup exe installer.  

## Project Evergreen
Project Evergreen AppTracker does not provide information and sources for installers for this app when last checked.


## SilentInstallHQ
Silent Install HQ provides information on the silent install of this app here: https://silentinstallhq.com/visual-studio-code-silent-install-how-to-guide/ .


## EXE based installer

Installer supports a silent installation:
* Use '/SP- /VERYSILENT /SUPRESSMSGBOXES /MERGETASKS=!runcode'

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* Preconfiguration is possibleby adding a `settings.json` file with desired settings.  This file is placed in the user AppData\Roaming\Code\User folder.  Some of the more common items to consider:
* * `"update.mode": "none"`  to disable the program autoupdates.
* * `"extensions.autoUpdate": false` to disable plugin extension updates.
* * `"telemetry.enableCrashReporter": false` to avoid sending Microsoft telemetry.
* * `"telemetry.enableTelemetry": false` to avoid sending Microsoft telemetry.
* * `"workbench.colorTheme": "Default Dark+"` because we can.

## Installed Components worth noting

* By default, the app installers components into the `Program Files`area.
* A configuration file may be placed in the AppData\Roaming folder if desired.
* 1 shortcut is installed by default.
* No FTAs, Shell Extensions, Protocol Handlers, or Services.
* The app adds 2 fonts.
