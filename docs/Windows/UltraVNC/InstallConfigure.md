# Installation and Configuration Notes for UltraVNC
By default the app will install under the apprpriate Program Files folder.

## Project Evergreen
Project Evergreen AppTracker does not provide information and sources for installers for this app when last checked.

## ZIP based installer

Is available, but not tested.

## EXE based installer

Supports silent installation, for example '/SILENT /VERYSILENT /LOADINF="xxx.inf".  Use '/?' for more options.
Here is a sample inf file:

```inf
[Setup]
Lang=en
Dir=C:\Program Files\uvnc bvba\UltraVNC
Group=UltraVNC
NoIcons=0
SetupType=full
Components=ultravnc_server,ultravnc_viewer,ultravnc_repeater
Tasks=installservice,associate,installdriver
```

## MSI based installer

Supports silent ('/qn') or passive ('/passive') options.

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* The product does not currently have an autoupdater built in.
* The product does not have any configuration settings.

## Installed Components worth noting

* The application installs with seven shortcuts (3 are duplicates on the desktop). One is a shortcut to the folder with the program. WIthout those there is a shortcut for the Server software, Client software, and Settings.
* The application has no FTA, Shell Extensions, or Protocol handlers.
* The application has a service (automatic start).
* The application places some installers in the %localappdata% are that are not required.
* On Windows 10 there is an optional component in the installer for a monitor driver.
