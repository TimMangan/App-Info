# Installation and Configuration Notes for WinRAR

The 64-bit version is recommended on 64-bit operating systems, which increases the maximum size of the compression archive.

## Project Evergreen
Project Evergreen AppTracker does not provide information and sources for installers for this app when last checked.


## SilentInstallHQ

Silent Install HQ provides information on the silent install of this app here: https://silentinstallhq.com/?s=WinRar .

## EXE Installation
The exe installer appears to use their own installer framework. A '/s' (lower case) provides for a silent installation.

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* None, except for default language if needed.
* Registry based pre-configuration is available.
* Repackaging techniques that involve recapture will only support a single language.  Some packaging forms allow for a script to be run on package installation or first run of the application.  In that case, adding additional launguage files in a side folder of the package could be used with a package script to detect the OS launguage and copy files appropriately. 

## Installed Components worth noting
 
* The application installs into program files.
* There are 4 shortcuts. The second is to a manual which is available from menu in the program. The third is a "What's New" link. The fourth is a help link.  Often these are removed.
* There  are lots of FTAs with shell extensions.  There are both Context Menus and Drop Handlers.  These are added to many zip like existing FTAs, new .rar* FTAs, and the special "*" FTA.
* There are no protocol handlers, or services.
* There is no autoupdater.
