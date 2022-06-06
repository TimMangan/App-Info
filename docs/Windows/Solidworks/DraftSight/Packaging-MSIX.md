# Packaging DraftSight for MSIX

TThe software was packaged on Windows 10 21H2 using Microsoft MSIX Packaging Tool 1.2022.512 with the PSF using TMEditX with the PSF FileRedirectionFixup.
* You must disable the Advertized Shortcuts for installation.
* Remove the unwanted shortcut from the desktop if desired.
* PsfLauncher is required for the shortcut in order to support the required command line argument.
* FileRedirectionFixup is recommended due to configuration files in the package that might be changed.
* TMEditX was used to add the Shell Extensions to the AppXManifest  Shared handlers are not supportable at this time so you may apply a given handler to only one file type.
* TMEditX was used to add in the missing fonts to the AppXManifest.


Testing on Windows 10/11 indicates ![badge](https://img.shields.io/badge/-Major%20Issues-critical?style=for-the-badge).

App crashes upon start.  Not diagnosed.


## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | June 2022 |


