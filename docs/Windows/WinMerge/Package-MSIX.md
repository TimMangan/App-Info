# Packaging WinMerge for MSIX

The software was packaged on Windows 10 21H2 using Microsoft MSIX Packaging Tool 1.2022.512 and TMEditX was used.
* The MMPT will, by default, ignore the shortcut to the help file. TMEditX will restore this using PsfLauncher.
* There are user customizations for things like colors.  These are ini and xml files in the program folder area. The PSF FRF was added.
* Missing ExecutionAlias entries were added to the manifest.



Testing on Windows 10/11 indicates ![badge](https://img.shields.io/badge/-Full%20Fidelity-brightgreen?style=for-the-badge) support of the app.



## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | June 2022 |

