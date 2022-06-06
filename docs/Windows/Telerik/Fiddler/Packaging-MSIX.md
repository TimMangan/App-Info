# Packaging Fiddler for MSIX

The software was packaged on Windows 10 21H2 using Microsoft MSIX Packaging Tool 1.2022.512 with the PSF using TMeditX.
* After install, import reg file with desired settings.
* Remove the uninst.exe from the program folder.
* While monitoring, run 'EnableLoopback.exe -All'
* PsfLauncher is required as is the RegLegacy, and EnvVar fixups.


Testing on Windows 10/11 indicates ![badge](https://img.shields.io/badge/-High%20Confidence-green?style=for-the-badge).


## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | April 2022 |


