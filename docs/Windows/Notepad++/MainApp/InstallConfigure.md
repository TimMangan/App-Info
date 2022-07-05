# Installation and Configuration Notes for Notepad++

By default the app will install into the user programs folder `Notepad++` by default.

## Project Evergreen
Project Evergreen AppTracker provides information and sources for installers for this app https://stealthpuppy.com/apptracker/#notepadplusplus 


## EXE based installer

The main exe installer supports silent installation. 
* Use '/S' for silent (must be a capital S).

The installer adds a shortcut to the start menu.


## SilentInstallHQ
Silent Install HQ provides information on the silent install of this app here: https://silentinstallhq.com/?s=Notepad%2B%2B.

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* Plugins are dlls that may be copied into a `PlugIns` folder under the main install.
* The product does have an autoupdater.  There are no installation options to disable it.  You can disable it in the GUI, and this will produce a set of XML files under AppData\Roaming\Notepad++.  This disable in the GUI isn't perminent, but you can edit the last checked date in the xml file to some distant future date for extended disablment.
* Adrian has posted some information on handling multiple languages when packaging for MSIX, however the technique is usable in other packaging scenarios as well.  See https://techcommunity.microsoft.com/t5/msix/notepad-automatic-language-configuration/m-p/3558411 


## Installed Components worth noting

* There is one shortcut.
* There is one FTA on the wildcard (*) with a Shell Extension Context Menu.
* The app installer does not write to AppData\Local or Roaming.