# Installation and Configuration Notes for AppV_Manage

By default the app will install into the user programs folder (x86) by default.


## MSI based installer

The main exe installer supports passive and silent installation. Some of the other options are documented https://www.tmurgent.com/appv/en/resources/AppV_Manage/225-appv-manage-installation. An example install might include:
``` ps1
 $args = '/passive'
 $args = $args + ' CONTENTUNC="\\nuc2\Packages"'
 $args = $args + ' FOLDERPARSINGLEVEL="4"'
 $args = $args + ' DEBUGLOGLEVEL="0"'
 $args = $args + ' USENEWGROUPFEATURES="1"'
 $args = $args + ' SETEXECUTIONPOLICYORIMPORT="0"'
 $args = $args + ' INSTALLSHORTBCUTSTARTMENU="1"'
 $args = $args + ' SKIPINSTALLSHORTCUTDESKTOP="1"'
 $args = $args + ' USEADVANCEDUI="0"'
 $args = $args + ' ROLEPUB="2"'
 $args = $args + ' ROLECLIENTPKG="1"'
 $args = $args + ' ROLECONGROUP="1"'
 $args = $args + ' ROLEDEBUGPKG="0"'
 $args = $args + ' ROLEPOWERSHELL="0"'
 $args = $args + ' ROLEEVENTS="1"'
 $args = $args + ' ROLEDEBUGEVENTS="2"'
 $args = $args + ' ROLETOOLCONFIG="1"'
 msiexec.exe /i Setup_AVM_5.17.0.0.msi $args
```

The installer adds a shortcut to the start menu.

## SilentInstallHQ
Silent Install HQ provides no information on the silent install of this app.

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* The product does not have an autoupdater.  It does have an obscure page that will show the new version available and allow the user to download it.


## Installed Components worth noting

* The application mostly uses the OS's built-in App-V Client and PowerShell module.
* The app installer does not write to AppData\Local or Roaming.