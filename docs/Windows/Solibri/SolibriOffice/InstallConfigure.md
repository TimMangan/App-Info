# Installation and Configuration Notes for Solibri Office

By default the app will install into the user programs folder by default.


## EXE based installer


The main exe installer uses a configuration file for silent installation. The file is well documented in the vendor's PDF.  
* Use '-q' for silent installation.
* Add "-console -varfile $($executingScriptDirectory)\response.varfile"

```varfile
# install4j response file for Solibri 9.12.7.24
createDesktopLinkAction$Boolean=false
executeLauncherAction$Boolean=false
resourceIndex$Integer=1
sys.adminRights$Boolean=true
sys.fileAssociation.extensions$StringArray="IFC","IFCzip","SMC","SMCT"
sys.fileAssociation.launchers$StringArray="118","118","118","118"
sys.installationDir=C\:\\Program Files\\Solibri\\SOLIBRI
sys.languageId=en
sys.programGroupAllUsers$Boolean=true
sys.programGroupDisabled$Boolean=false
sys.programGroupName=Solibri
```

The installer adds two shortcuts to the start menu, one for the product and one for an uninstaller  Often removing the uninstall shortcut ('Solibri Uninstaller.lnk') is desired.

## SilentInstallHQ
Silent Install HQ provides no information on the silent install of this app.  

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

## Installed Components worth noting

* The app has .cfg and .xml files under the installation folder.
* The app adds .xml files into the C:\Users\Public\SOLBRI\Roles folder.
* The app adds 4 new FTAs with Shell command verb integrations.
* No Shell extensions, protocols, or services.
