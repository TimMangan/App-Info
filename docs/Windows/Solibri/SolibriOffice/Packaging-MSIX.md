# Packaging Solibri Office for MSIX

The software was packaged on Windows 10 21H2 using Microsoft MSIX Packaging Tool 1.2022.512 with the PSF using TMEditX.
* PSFLauncher,  FileRedirectionFixup and DynamicLibraryFixup are needed.
* TMEditX was used to add FONTS into the AppXManifest.



Testing on Windows 10/11 indicates ![badge](https://img.shields.io/badge/-Major%20Issues-critical?style=for-the-badge).

The app includes a copy of a Java JRE, however it isn't being found by the app when launched in the container.  This needs more investigation, but seems like it is the known runtime issue with the registry. 


## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | June 2022 |


