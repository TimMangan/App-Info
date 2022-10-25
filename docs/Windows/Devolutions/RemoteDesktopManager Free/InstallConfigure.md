# Installation and Configuration Notes for Remote Desktop Manager (free)

By default the exe installer for this app will install into folder under  `Program Files (x86)\Devolutions\Remote Desktop Manager Free`. 

## Project Evergreen
Project Evergreen AppTracker does not provide information and sources for installers for this app when last checked.


## MSI based installer
The MSI installer appears to only have the typical MSI options.




## SilentInstallHQ
Silent Install HQ provides no information on the silent install of this app.
## Typical Configuration Items 
The application has an update detector.  This may be defeated by using a preconfigured file and adding it into the installation folder.  You can use the UI to configure everything that you want, then extract the "RemoteDesktopManagerFree.cfg" file and adding this into the deployment.  Sites and passwords are stored in other areas.  To manually add the entry to this file, use:

  <UseDevolutionsUpdate>false</UseDevolutionsUpdate>

## Installed Components worth noting
* The app installs into Program Files (X86).
* There is one shortcut for the app plus another .url for help.
* There are no FTAs, but there is a URL (rdm).
* There are no Shell Extensions or Services, but lots of COM.
