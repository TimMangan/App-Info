# Installation and Configuration Notes for Password Depot

By default the app will install under a `AceBit` folder in the Program Files folder.


## EXE based installer

The EXE installer supports a lot of switches, including one to disable updates.  For example, use 
* '/SP- /SILENT /SURPRESSMSGBOXES /UpdateMode=2'.


## SilentInstallHQ

Silent Install HQ provides no information on the silent install of this app.

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* None identified

## Installed Components worth noting
 
* No files in AppData/Local or Roaming by the installer.
* There is a desktop shortcut installed that is commonly removed.
* There are 3 start menu shortcuts.  One for the product, one for a 'Virtual Keyboard', and one for 'uninstall'. The uninstall is commonly removed.
* There is an updater, enabled by default.  This may be turned off through a file in the user's appdata\local folder. Unfortunately, the software generates a system hash for the path to this file so automated packaging to turn this off is not pratical except by end-user.  But this is the same as with a native install.
* FTA with Shell Extension Context Menu for '*' and 'Directory'.
* FTA with Shell Integration Verb Command for .pwde and .pwdz
* The installer adds an ini file in the installation directory.
