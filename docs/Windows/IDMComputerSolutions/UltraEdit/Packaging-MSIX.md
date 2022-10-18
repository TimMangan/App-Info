# Packaging UltrEdit for MSIX

The software was packaged on Windows 10 21H2 using Microsoft MSIX Packaging Tool 1.2022.330 and enhanced by editing with TMEditX to inject the PSF.1

In the MMPT:
* After app install, copy configuration file (`uedit64u.ini`) with desired settings under the logged in user's AppData\Roaming\IDMComp\UltraEdit folder.
* If this file is added, you must also create the folder AppData\Roaming\IDMComp\UltraEdit\volatile (and either place a dummy file in it or let the MMPT create one for you).  Otherwise the end-user will get a popup error on first run that it can't create the folder.
* The product installs PRogIDs, but you have to run the product and use file->settings to apply the FTAs.  We solved this without launching during capture by using a reg file (running an installed copy and exporting the FTA to create reg file, shown below) during this capture.
* Four COM objects are ignored by the MMPT because the app did not register the ProgID in the exact form the MMPT exptected.  Clearly the base OS didn't mind this, but the MMPT does. We overcome this by importing an additional reg file:

```reg```
Windows Registry Editor Version 5.00


[HKEY_LOCAL_MACHINE\SOFTWARE\Classes\CertMng.CertStores\CurVer]
@="CertMng.CertStores.1"

[HKEY_LOCAL_MACHINE\SOFTWARE\Classes\CertMng.Certificates\CurVer]
@="CertMng.Certificates.1"

[HKEY_LOCAL_MACHINE\SOFTWARE\Classes\WeOnlyDo.DirItem\CurVer]
@="WeOnlyDo.DirItem.1"


[HKEY_LOCAL_MACHINE\SOFTWARE\Classes\WeOnlyDo.DirItems\CurVer]
@="WeOnlyDo.DirItems.1"

```

In TMEditX
* PsfLauncher is required as is the FRF.
* Several Shell commands are missing for the fta in the manifest as MMPT supports only one verb per FTA.  TMEditX can fix this.
* LoaderSearchOrder fix to manifest is warrented. TMEditX can fix this.
* ExecutionAlias fix to manifest is warrented.  TMEditX can fix this.

```reg
Windows Registry Editor Version 5.00

[HKEY_CURRENT_USER\Software\Classes\*\OpenWithList\uedit64.exe]
@=""

[HKEY_CURRENT_USER\Software\Classes\*\shellex\ContextMenuHandlers\UltraEdit]
@="{b5eedee0-c06e-11cf-8c56-444553540000}"

[HKEY_CURRENT_USER\Software\Classes\Applications\uedit64.exe]

[HKEY_CURRENT_USER\Software\Classes\Applications\uedit64.exe\shell]

[HKEY_CURRENT_USER\Software\Classes\Applications\uedit64.exe\shell\edit]

[HKEY_CURRENT_USER\Software\Classes\Applications\uedit64.exe\shell\edit\Command]
@="\"C:\\Program Files\\IDM Computer Solutions\\UltraEdit\\uedit64.exe\" \"%1\""

[HKEY_CURRENT_USER\Software\Classes\Applications\uedit64.exe\shell\open]

[HKEY_CURRENT_USER\Software\Classes\Applications\uedit64.exe\shell\open\Command]
@="\"C:\\Program Files\\IDM Computer Solutions\\UltraEdit\\uedit64.exe\" \"%1\""

[HKEY_CURRENT_USER\Software\Classes\Applications\uedit64.exe\shell\print]

[HKEY_CURRENT_USER\Software\Classes\Applications\uedit64.exe\shell\print\Command]
@="\"C:\\Program Files\\IDM Computer Solutions\\UltraEdit\\uedit64.exe\" /p \"%1\""

[HKEY_CURRENT_USER\Software\Classes\CLSID\{b5eedee0-c06e-11cf-8c56-444553540000}]

[HKEY_CURRENT_USER\Software\Classes\CLSID\{b5eedee0-c06e-11cf-8c56-444553540000}\InProcServer32]
@="C:\\Program Files\\IDM Computer Solutions\\UltraEdit\\ue64ctmn.dll"
"ThreadingModel"="Apartment"

```


Testing on Windows 10/11 indicates ![badge](https://img.shields.io/badge/-Full%20Fidelity-brightgreen?style=for-the-badge).  


## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | April 2022 |


