# Packaging Anaconda for MSIX

The software was packaged on Windows 10 21H2 using Microsoft MSIX Packaging Tool 1.2022.330 and enhanced by editing with TMEditX to inject the PSF.
* The [{Personal}] folder exclusion should be removed from all tooling before repackaging.
* PsfLauncher is required as is the FRF.

Testing on Windows 10/11 indicates ![badge](https://img.shields.io/badge/-Major%20Issues-critical?style=for-the-badge).  These issues were from the use of the Microsoft MSIX Packaging Tool; perhaps other tooling will work.



## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | April 2022 |

