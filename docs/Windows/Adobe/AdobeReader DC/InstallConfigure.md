# Installation and Configuration Notes for AdobeReader DC
By default the app will install into a `Adobe` folder under the apprpriate Program Files folder.

To distribute this product inside your organization, you are required to register for this purpose (free).  This registration makes the Abobe Customization Wizard available to you, as well as the MSI based installer.

## Project Evergreen
Project Evergreen AppTracker provides information and sources for installers for this app https://stealthpuppy.com/apptracker/#adobeacrobatdc  


## MSI based installer

Use the Customization Wizard to generate a MST file. Normal MSI parameters are available for quick/passive/silent installation.  By default, the installation uses Advertized Shortcuts, which should normally be disabled when repackaging into forms other than another MSI.

## SilentInstallHQ
Silent Install HQ provides information on the silent install of this app https://silentinstallhq.com/?s=Adobe+Reader+DC

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* The product has an autoupdater built in that may be disabled.
* Use the Customization Wizard to configure this and all other settings.

## Installed Components worth noting

* The application installs with one shortcut. 
* The install includes 9 FTAs.
* There is one shell extension, a preview handler.
* There are 11 ActiveX components.  With IE11 going away, these may not be important any more.
* There is one URL handler.
* There is one service, however it is disabled and not needed if the updates are disabled.
* There are 16 fonts.
* There is an AppPaths registration.
* The installed app does not use AppData local or roaming folders.