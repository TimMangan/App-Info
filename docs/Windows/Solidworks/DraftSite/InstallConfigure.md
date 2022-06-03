# Installation and Configuration Notes for DraftSite

By default the app will install into the user programs folder by default.


## EXE based installer

Extract the files from the provided exe:
* Use '/Q /T:"C:\Extract" /C ' to extract the actuall installer.

To continue with the extracted version of the exe installer,
* Use '/s ' for silent installation.  It has an embedded MSI, so for full silent installation, use '/s /v/qn'.

The installer adds a shortcut to the start menu and to the desktop.  Often removing the desktop shortcut is desired.

## MSI based installer
* Use '/qn' for silent installation.  It has an embedded MSI, so for full silent installation, use '/qn DISABLEADVTSHORTCUTS=1'.
* Use '/passive' for silent installation.  It has an embedded MSI, so for full silent installation, use '/passive DISABLEADVTSHORTCUTS=1'.

The installer adds a shortcut to the start menu and to the desktop.  Often removing the desktop shortcut is desired.

## SilentInstallHQ
Silent Install HQ provides no information on the silent install of this app.  

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* The product does not have an autoupdater.
* Other customizations were not tested.

## Installed Components worth noting


* It installs under Program Files
* It installs files to ProgramData
* It installs files to C:\Application Data\...
* The Shortcut to the program includes a command line argument "/IA".
* It has 2 services, a DraftSite API Service and a Flexnet Licensing Service.
* It has several FTAs and shell extensions:
* * .dwg, .dwt, with shared Preview Handler and shared Thumbnail Handler.
* * .dxf with Preview Handler and Thumbnail Handler.
* * .flx with Preview Handler and Thumbnail Handler.