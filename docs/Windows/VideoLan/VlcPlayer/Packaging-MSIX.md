# Packaging VlcPlayer for MSIX

The software was packaged on Windows 10 21H2 using Microsoft MSIX Packaging Tool 1.2022.512 and TMEditX was used to fix up the package:

MMPT:
* It is necessary to remove unwanted shortcuts while in monitoring mode.  The MMPT becomes confused due to the same start names 'VLC media player' and 'VLC media player - reset preferences and cache files'.
TMEditX:
* PsfLauncher and FileRedirectionFixup will be needed.
* Missing FTA Shell Verb commands restored.
* 2 missing fonts restored.
* LoaderSearchOrder and ExecutionAlias added.



Testing on Windows 10/11 indicates ![badge](https://img.shields.io/badge/-Full%20Fidelity-brightgreen?style=for-the-badge) support of the app.


## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | June 2022 |

