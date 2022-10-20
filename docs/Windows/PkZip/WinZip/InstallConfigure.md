# Installation and Configuration Notes for WinZip

By default the app will install in the Program Files folder.

## Project Evergreen
Project Evergreen AppTracker provides no information and sources for installers for this app. 

## SilentInstallHQ

Silent Install HQ provides this information on the silent install of this app: https://silentinstallhq.com/?s=Winzip.

## EXE based installer

The EXE installer supports a silent installation. It includes the MSI and options for the msi may be added as shown in the example below:
    '/exenoui /qn ADDDESKTOPICON=0, ISCHECKFORUPDATES=0, NOPRODADVUPDATES=1'

See the MSI section for regarding additonal MSI options.

Ultimately, many of these options will be stored in the registry.  For example, the autoupdate check may be disabled after install with a .reg file import as shown here:

```reg
Windows Registry Editor Version 5.00

[HKEY_LOCAL_MACHINE\SOFTWARE\Nico Mak Computing\WinZip\UpdateCheck]
"NoUpdateChecking"="0"
```

## MSI based installer
Both quiet ('/q') and passive ('/passive') options are available.  Additionally, there are a ton or properties available in the MSI Properties table for customization during install.  Here are a few of these properties that may be of interest:

| Property | Default | Common | Why |
|----|----|----|-----|
| ISCHECKFORUPDATES | 1 | 0 | Disable update check. |
| LAUNCHPROGRAM | 1 | 0 | Keeps installer from starting app when done. |
| AgreeToLicense | No | Yes | Accept Eula for user. |
| ADDDESKTOPICON | 1 | 0 | Prevent icon from being installed on desktop. |
| ALLLANGS | 0 |   | 1 to install all languages so you can deploy to different OS langs. |
| DISABLEADVTSHORTCUTS | 1 | 1 | Not appropriate for containerized apps, but MSI repackaers usually like this set to 0. |
| ENABLEEXPRESSFEATURES | 1 |   | Unknown. |
| INSTALLEXPRESSOFFICE | 1 |   | Unknown. |
| FIPSCOMPLIANCEMODE | DISABLED |   | ENABLED to turn this on where needed (Security). |
| DISABLESHAREDFILES | 0 |   | 1 to disable where needed (Security). |
| ALWAYSENCRYPT | DEFAULT |   | Probably set to 1 where needed (Security). |
| DEFAULTCOMPRESSIONMETHOD | 1 |   | Because you can. |

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* In addition to the desktop shortcut that you can turn off in the installer, two additional start menu shortcuts are added that are typically not wanted. 'Update Notifier' and 'WinZIP Background Tools'.  This version also includes a number of other shortcuts which removal should be considered based on local needs.

## Installed Components worth noting
 
* The application installs into Program Files.
* The app installs one file under the user AppData/Local folder (it might not need to be recaptured).
* There are many FTAs with multiple Shell Integration Verb commands each, and Shell Extensions.
* The FTA Shell Extensions include Context Menu, Drop Handler, and Preview Handler handlers are installed, including both standard file types (like '.zip'), but special types including '*', 'Directory', 'Folder', and 'Drive'
* There is a Protocol Handler 'WzExpForSPExtension' which is possibly used in SharePoint scenarios.
* There is a 'WinZip Preloader.lnk' shortcut added to the Common Startup folder.  It points to an exe that appears to be used to aid performance, but the product appears to be OK even without it.
