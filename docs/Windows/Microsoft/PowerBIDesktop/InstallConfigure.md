# App-Info Install/Configure for Power BI Desktop

The application is delivered in a setup exe installer.  

## Project Evergreen
Project Evergreen AppTracker does not provide information and sources for installers for this app when last checked.


## EXE based installer

* Use `-q` for silent or `-passive` for a passive installation.
* To accept the EULA, use `ACCEPT_EULA=1`
* To disable updates, use `DISABLE_UPDATE_NOTIFICATION=1`

## SilentInstallHQ
Silent Install HQ provides no information on the silent install of this app.

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.   This application uses both HKLM and HKCU registry items:

* `HKLM\SOFTWARE\Microsoft\Microsoft Power BI Desktop\DisableUpdateNotification 	DWORD 1` is the option set by the installer option to disable updates.
* `HKCU\Software\Microsoft\Microsoft Power BI Desktop\ShowLeadGenDialog			DWORD 1`
* `HKCU\Software\Microsoft\Microsoft Power BI Desktop\EnableCustomerExperienceProgram	DWORD 0`
* `HKCU\Software\Microsoft\Microsoft Power BI Desktop\Installer\InstallDesktopShortcutValue	DWORD 0`

The product installs a shortcut both to the start menu and desktop.  There is no installer option to avoid the desktop short.  If removed, the product will add the desktop shortcut back unless the InstallDesktopShortcutValue registry setting is set to 0.



## Installed Components worth noting

* By default, the app installers components into both the `Program Files` and `Program Files (x86)` folders.
*  2 shortcuts are installed by default. One is in the start menu, the other to the desktop.  Both point to the same exe.
* 3 FTA for app specific file types, with Shell Integration Command.
* No Shell Extensions, or Services.
* 1 new Protocol Handler.
* The app installer does not create folders in the User's AppData\Roaming area.
* The app at runtime uses the user's AppData\Local\Temp folder.
