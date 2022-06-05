# Installation and Configuration Notes for CyberDuck

By default the exe installer for this app will install into several folders under both Program Files and Program Files (x86). In both, there are both a Bonjour folder and a CyberDuck folder.

## Project Evergreen
Project Evergreen AppTracker provides information and sources for installers for this app https://stealthpuppy.com/apptracker/#cyberduck 



## MSI based installer
The MSI installer appears to only have the typical MSI options.

The MSI version of the installer seems to skip the Bonjour service installation (even though files are in the package).

## EXE based installer

The exe based installer support both silent and passive install, but no other options have been found.

* Use `/Install /quiet` for silent.
* Use `/Install /passive` for passive.


## SilentInstallHQ
Silent Install HQ provides information on the silent install of this app https://silentinstallhq.com/?s=CyberDuck

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* While preconfiguration is possible, I'd recommend avoiding it on this app.
* Preconfiguration customizations were not tested.

## Installed Components worth noting

* The application includes installing the Apple Bonjour service. This could be disabled or removed if not needed.  See the Program Files (x86)\Bonjour folder for documentation on what this service is for.
* The application installs with one shortcut. 
* The app has 3 FTAs and a slew of Protocol Handlers.
* The app does not install files into the user's AppData\Local or Roaming folders, however user configuration file will be written to the Roaming folder by the runtime application.