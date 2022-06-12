# Installation and Configuration Notes for Zoom Client
By default the app will install under the apprpriate Program Files folder.

## Project Evergreen
Project Evergreen AppTracker provides information and sources for installers for this app here: https://stealthpuppy.com/apptracker/#zoom.

## SilentInstallHQ
Silent installation information is not available from SilentInstallHQ for this app at this time.

## MSI based installer

Supports silent ('/q') and passive (/passive) installations. 


## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* The MSI installer installed into Program Files (x86).
* The installer adds an extra shortcut to the desktop.

## Installed Components worth noting

* The application installs with one shortcut in the start menu and another on the desktop. 
* The application has a service which is needed if you want others to be able to remote control this client's desktop (with permission, of course).
* The installer writes some files to the AppData\Roaming folder for the user as placeholders.  This folder may be removed from the package if it is desired to keep the applications appdata use external to a container (MSIX for example).
* There are ini and xml files in the Program Files area which might possibly be written to.
* The application has no shell extensions. 
* The application has numerous protocol handlers.