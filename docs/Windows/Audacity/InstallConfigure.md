# Installation and Configuration Notes for Audacity
By default the app will install into a `Audacity` folder under the apprpriate Program Files folder.

## Exe based installer

Silent installation is possible:  

* "/SP /VERYSILENT /SUPPRESSMSGBOXES" (capitalized) for silent installation. 
* A preconfigured audacity.cfg file may be copied into the AppData\Roaming folder.

## SilentInstallHQ
Silent Install HQ provides information on the silent install of this app https://silentinstallhq.com/?s=Audacity

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* The product currently has an autoupdater built in.
* File based configuration available under AppData\Roaming

## Installed Components worth noting

* The application installs with two shortcuts, one for the desktop and another for the start menu.  Desktop shortcut is commonly removed.
* The application adds one FTA (.aup).
* The installed app does use AppData\Roaming and \Local folders.