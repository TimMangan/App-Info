# Packaging R (Language) for MSIX

The software was packaged on Windows 10 21H2 using Microsoft MSIX Packaging Tool 1.2022.512 with the PSF using TMEditX.
* Only the PSfLauncher is needed, because there are both 32 and 64-bit exes with the same name that need a shortcut.

The application attempts to install an FTA on .RData with a shell integration verb command using the same 'open' verb to start the 32 and 64 bit RGui.exe, one on .rdata and other on .RData.  MSIX cannot handle this and you must choose one or the other, but usually this means the 64 bit version.


Testing on Windows 10/11 indicates ![badge](https://img.shields.io/badge/-Full%20Fidelity-brightgreen?style=for-the-badge).  
 


## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | April 2022 |


