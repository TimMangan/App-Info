# Installation and Configuration Notes
By default the app will install into a `C:\Python3x` folder under the apprpriate Program Files folder.

## MSI based installer

Normal MSI parameters are available for quick/passive/silent installation.

## SilentInstallHQ
Silent Install HQ provides information on the silent install of this app https://silentinstallhq.com/?s=ActivePython 

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* The product does not currently have an autoupdater built in.
* The product does not have any configuration settings needed as the developer will set up their environment post-installation.

## Installed Components worth noting

* The application installs with four shortcuts. One is to a cmd prompt, one is to the python.exe interactive shell, the other two are cmd/bat files.
* The install includes an AppPaths registration and change to the Path environment variable.
* The installed app does not use AppData local or roaming folders, however the runtime will use the temp folder for temporary storage.