# Packaging WinRAR for MSIX

The software was packaged on Windows 10 21H2 using Microsoft MSIX Packaging Tool 1.2022.330 with or without PSF using TMEditX.
* PsfLauncher is required if the additional shortcuts to the read me or what's new or manual are left in the package.
* PsfLauncher and RegLegacyFixup are needed. There is an issue with being able to set and save some registry configuration.  The FRF is not required if WinRAR is not used multilingually.
If multiple languages are to be supported, the language files "*.lng" must be redirected via FRF and the corresponding "*.lng" files of the language must be copied into the FileRedirection path via Powershell Startup script.

* Missing LoaderSearchOrder and ExecutionAlias are added into the manifest.

Testing on Windows 10 indicates ![badge](https://img.shields.io/badge/-Mostly%20Works-yellow?style=for-the-badge) Support of the app.  This is due to missing Shell Context Menu which is pretty important to many users for this app.

Testing on Windows 11 indicates ![badge](https://img.shields.io/badge/-Mostly%20Works-yellow?style=for-the-badge) support of the app.  Although the context menus look correctly formed in the manifest, they are not working.  Additionally, the open with like FTA for the app is now missing...


## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | June 2022 |

