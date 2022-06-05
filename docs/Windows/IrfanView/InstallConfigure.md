# Installation and Configuration Notes for IrfanView

By default the app will install under a `IrfanView` folder in the Program Files folder.

## Project Evergreen
Project Evergreen AppTracker does not provide information and sources for installers for this app when last checked.


## EXE based installer

The main exe installer supports passive installation:
* For example, use  "/silent /folder=`"c:\Program Files\irfanview`" /desktop=0 /thumbs=1 /group=1 /allusers=0 /assoc=1 /ini=`"$($env:APPDATA)\irfanview`"" 
* Remove the desktop shortcut.
* Optionally copy pre-pared igconfig.xml and igstartup.profile file to the AppData/Roaming/ImageGlass folder.

## Plugin Installer
Here is an exmple of installing a plugin:
* iview458_plugins_x64_setup.exe"   /silent /folder="c:\Program Files\irfanview"
    

## SilentInstallHQ
Silent Install HQ provides information on the silent install of this app at https://silentinstallhq.com/?s=Irfanview.

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* The i_view64.ini file (i_view32 on 32bit installs) is the general configuration file. It goes into the user's AppData\Roaming\IrfanView folder.
* Two additional shortcuts are placed on the desktop and are commonly removed as part of repackaging.


## Installed Components worth noting

* The application itself  uses the AppData\Roaming  folders. 
* There are ~75 FTAs none of which set IrfanView as the default.  
* There are no Shell Extensions, URL Handlers, or Services.
