# App-Info Install/Configure for SSMS

The application is delivered in a setup exe installer.  

## Project Evergreen
Project Evergreen AppTracker does not provide information and sources for installers for this app when last checked.


## EXE based installer

Installer supports a silent installation:
* Use '/Install' with either '/Passive' or '/Quiet'
* To Specify a different installation folder: '/SSMSInstallRoot=<path to install>'

## SilentInstallHQ
Silent Install HQ provides no information on the silent install of this app.

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* While preconfiguration may be possible, given the limted but experienced set of users for this app, it is usually installed unconfigured.  Some communtity driven ideas on configuring the app may be found here: https://www.mssqltips.com/sql-server-tip-category/261/sql-server-management-studio-configuration/
* The gui has the ability to export/import a configuration file as well.

## Installed Components worth noting

* By default, the app installers components into both the `Program Files` and `Program Files (x86)` folders.
*  4 shortcuts are installed by default.
* 14 FTA, with Shell Integration Commands.
* No Shell Extensions, Protocol Handlers, or Services.
* The app has an ETW provider.
* The app adds the PATH variable.
* The app installer creates folders in the User's AppData\Roaming area.
* The app installer adds folders and files to the user's AppData\Local folders.
