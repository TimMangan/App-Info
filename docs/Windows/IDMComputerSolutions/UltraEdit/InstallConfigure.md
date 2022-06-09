# Installation and Configuration Notes for UltraEdit

By default the app will install into the user programs folderby default.

## MSI based installer
AN MSI installer is directly available from the vendor.  It supports the common MSI parameters.

## EXE based installer

The exe installer embeds an msi installer supports passive and silent installation:
* '/s /v"qn"' for silent.
* '/s /v"passive"' for passive.

The installer adds a shortcut to the start menu.

## SilentInstallHQ
Silent Install HQ provides information on the silent install of this app at this link: https://silentinstallhq.com/?s=UltraEdit 

## Typical Configuration Items 

The application uses an ini file, 'uedit64u.ini', that is placed in the user's AppData/Roaming/IDMCOMP/UltraEdit folder.  

Preconfiguration of the app may be performed by including this file in the package.  Change line to 'Check For Updates=0' to disable update checks.



## Installed Components worth noting

* The app adds 4 shortcuts, 3 to the main program and one for the uninstaller.
* It is normal to remove the desktop and quick launch versions of the main program and also the uninstaller.
* There are no shell extensions, protocol handlers, or services.
* The product has xml files in the installation area; it is unclear if these might change in use.
* The configuration is a file under AppData\Roaming.