# Packaging Filezilla for MSIX

The software was packaged on Windows 10 21H2 using Microsoft MSIX Packaging Tool 1.2022.330 and enhanced by editing with TMEditX to inject the PSF.
* After install, copy xml file with desired settings under AppData\Local.
* Remove unnecessary shortcut to `Uninstall`.
* PsfLauncher is required as is the RegLegacy, and EnvVar fixups.


Testing on Windows 10/11 indicates ![badge](https://img.shields.io/badge/-Full%20Fidelity-brightgreen?style=for-the-badge).  


## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | April 2022 |


