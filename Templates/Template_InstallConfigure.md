# App-Info Install/Configure Template

The InstallConfigure markup file for an application should:
* Identify the key command line arguments typically used for installing this app from the vendors installer.  
* * If the vendor offers both exe and msi installers, each should be covered.
* * A silent or passive install is usually appreciated.
* * When possible, a link to SilentInstallHQ is appreciated.
* Identify the typical configuration items of interest when organizations pre-configure the application for end-users.  The information provided is usually used in repackaging operations to build a customized package.
* Document the "interesting" components installed.  Some repackaging technologies may have difficulties with some of these and the verification testing will look for them.  This includes:
* * Shortcuts
* * File Type Associations
* * FTA associated Shell Integration Commands
* * FTA associated Shell Extensions
* * Protocol handlers
* * Services
* * If the installer adds files to AppData/Local or Roaming or Documents.

Remove the boilerplate above this line.
____

# Installation and Configuration Notes for XXX

The application is delivered in a setup exe or MSI installer. By default it installs to the Progam Files area.  


## Project Evergreen
Project Evergreen AppTracker does not provide information and sources for installers for this app when last checked.
or 
Project Evergreen AppTracker provides information and sources for installers for this app https://stealthpuppy.com/apptracker/#... 


## EXE based installer

Installer supports a silent installation:
* Use '/silent'

## MSI Based installer
The installer supports the use of the standard MSI command line parameters.

## SilentInstallHQ
Silent Install HQ provides no information on the silent install of this app.

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* The Autoupdater is turned off (how if not covered in installer example).
* Several of the shortcuts might be removed, such as uninstaller and shortcuts to websites (identify)
* Preconfigured files or registry settings of interest.

## Installed Components worth noting

* XXX shortcuts are installed by default.
* X FTA (.XXX) with Shell Integration Command
* No Shell Extensions, Protocol Handlers, or Services.
* The app installer does not install anything in the user's AppData\Local or Roaming folders.
