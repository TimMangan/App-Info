# Installation and Configuration Notes for Libre Office

By default the app will install under a `Filezilla` folder in the Program Files folder.


## MSI based installer

The mai installer supports normal options for installation which includes the ability to turn off autoupdates.  For example, 
* '/qn /norestart ALLUSERS=1 CREATEDESKTOPLINK=0 REGISTER_ALL_MSO_TYPES=0 REGISTER_NO_MSO_TYPES=1 ISCHECKFORPRODUCTUPDATES=0 QUICKSTART=1 ADDLOCAL=ALL UI_LANGS=en_US,fr,es /l "c:\Users\Public\Documents\SequencedPackage\libreoffice.log'


## SilentInstallHQ
Silent Install HQ provides this information on the silent install of this app: https://silentinstallhq.com/?s=Libre+Office 

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* The application uses a registry based configuration. None were used in this test, other than as shown in the example MSI install command options.
* Other customizations were not tested.

## Installed Components worth noting

* The application install does not use the AppData\Local or Roaming folders. 
* Eight shortcuts are added by default.
* ~125 FTAs are added/modified.  With a lot of shell extensions.
* There is one protocol handler.
* There are no services.
