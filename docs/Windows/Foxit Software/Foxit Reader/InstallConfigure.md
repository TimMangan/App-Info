# Installation and Configuration Notes for Foxit Reader

By default the app will install under a `Foxit Software\Foxit PDF Reader` folder in the Program Files (x86) folder.

## Project Evergreen
Project Evergreen AppTracker provides information and sources for installers for this app https://stealthpuppy.com/apptracker/#foxitreader 

## EXE based installer
Available, but the Enterprise installer is the same software but more easily dealt with.

## MSI based installer

The main exe installer supports silent/passive installation:

* See https://cdn01.foxitsoftware.com/pub/foxit/manual/reader/en_us/FoxitReaderDeploymentAndConfiguration12.0_Manual.pdf
* Use  '/qn' for silent installation, /passive for passive. More options clearly documented in the above PDF
* Install any plugins.
* Copy the profstore.xml file to the program directory.
* Remove unnecessary shortcut to `Uninstall Foxit PDF Reader` and `Activate Plugins`.
* Disable the windows service `FoxitReaderUpdateService` which is obviously for autoupdating. Also an editor for that xml file.

Note that their is a customization wizard, MSTs for languages, and it is configurable via GPO.  See manual.pdf above for details.

## SilentInstallHQ
Silent Install HQ provides this information on the silent install of this app: https://silentinstallhq.com/?s=foxit+reader 

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* The application uses an xml file for the configuration. You can make this file with a test install that you configure.  Copy the file from the profstore.xml file from installation folder to copy to target systems with the plugins activated.
* The product does have an autoupdater. Disable the service.

## Installed Components worth noting

* The application install uses the AppData\Roaming folder. 
* There are 6 FTAs, each has 3 shell integration commands.
* There are three Shell Extensions (Thumbnail, Preview/PreviewHost, and an ActiveX that seems like it might be for sharepoint).
