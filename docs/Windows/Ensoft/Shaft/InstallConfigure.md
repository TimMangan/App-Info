# Installation and Configuration Notes for Ensoft Shaft

By default the app will install into the user programs folder by default.


## EXE based installer


The main exe installer supports passive installation:
* Use '/silent /hide [EULA_accept]=Yes /[License]=single'.

The installer adds a shortcut to the start menu to uninstall that should be removed.

## SilentInstallHQ
Silent Install HQ currently provides no information on the silent install of this app.

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* The product does not have an autoupdater.
* The product does have a dongle license, we are testing in 'demo mode' without it.

## Installed Components worth noting

* The application install uses both AppData\Local and AppData\Roaming folders. 
* There is one FTA (.sf8d) but no shell extensions.