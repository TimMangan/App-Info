# Installation and Configuration Notes for Audacity
By default the app will install into a `Audacity` folder under the apprpriate Program Files folder.

## Project Evergreen
Project Evergreen AppTracker provides information and sources for installers for this app https://stealthpuppy.com/apptracker/#audacity 

## Exe based installer

Silent installation is possible:  

* "/SP /VERYSILENT /SUPPRESSMSGBOXES" (capitalized) for silent installation. 
* "/SP /SILENT /SUPPRESSMSGBOXES" (capitalized) for passive installation. 
* A preconfigured audacity.cfg file may be copied into the AppData\Roaming\Audacity folder.
* Additional preconfig files are needed to be copied there if you want to register ffmpeg.

## FFMPEG
See instructions from audacity, but there is a zip file that contains a dll.  You can unpack this whereever you want (I suggest C:\Program Files\Audacity\FFMPEG folder) and
then register this location in the edit->preferences menu of the app.  Be sure to make other changes and then save off the entire AppData\Roaming\Audacity folder (except file the log)
and copy that out after installs.

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
