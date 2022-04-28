# Installation and Configuration Notes for ConEmuPack
By default the app will install into a `ConEmu` folder under the apprpriate Program Files folder.


## EXE based installer

* For the 64-bit version use '/p:x64'
* For silent installation use '/qn'

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* The product has an update detector built in.
* Configuration is stored in an xml file in the user's AppData\Roaming folder (not under a subfolder).
* You might want to remove the duplicate desktop shortcut.

## Installed Components worth noting

* The application uses AppData\Roaming.
* There is an update detection that may be configured off in the xml based configuration file.