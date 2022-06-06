# Packaging Password Depot for MSIX

The software was packaged on Windows 10 21H2 using Microsoft MSIX Packaging Tool 1.2022.330 with or without PSF using TMEditX.
* The PsfLauncher and FRF are needed (file based configuration in Program Files).
* It is necessary to keep shell extensions out of the package manifest due to duplicate guid issues.  It is unclear if these are really needed.


Testing on Windows 10/11 indicates ![badge](https://img.shields.io/badge/-High%20Confidence-green?style=for-the-badge) due to missing Context menu.  
 


## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | April 2022 |


