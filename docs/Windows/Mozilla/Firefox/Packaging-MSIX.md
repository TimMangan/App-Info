# Packaging Firefox for MSIX

`NOTE`: Firefox is now available from the Microsoft Store.  However creating your own customized package is also possible when you don't want to use the Microsoft Store.

The software was packaged on Windows 10 21H2 using Microsoft MSIX Packaging Tool 1.2022.330 without PSF.
* During the install, the maintenance service was disabled.  It may be advantagious to remove this unnecessary service while in monitoring mode.  Otherwise, the AppXManifest will be marked for the service capability and elevation is needed when manual installation of this package is performed by a standard user (but typically not an issue for software deployment tools)
* Although the package has many ini and xml files, these are not routinely changed during production use of the software, so the FRF is not needed.
* PsfLauncher is required as is the RegLegacy, and EnvVar fixups.


Testing on Windows 10/11 indicates ![badge](https://img.shields.io/badge/-Mostly%20Works-yellow?style=for-the-badge).  



## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | April 2022 |

