# Packaging SnagIt for MSIX

The software was packaged on Windows 10 21H2 using Microsoft MSIX Packaging Tool 1.2022.512 with the PSF and FileRedirectionFixup using TMeditX.
* FileRedirectionFixup might be needed to enable writing to a wide variety of ini and xml files.
* TMEditX was used for the following fixups to the package produced by the MSIX Packaging Tool:
* * Context Menus (you may choose to fix either "*" or "Directory" but not both due to AppXManifest limitations).
* * Image Handler.
* * Missing Fonts.
* * ExecutionAlias for Snagit32.exe.



Testing on Windows 10/11 indicates  ![badge](https://img.shields.io/badge/-Major%20Issues-critical?style=for-the-badge).  The application includes a component, SnagPriv.exe, that is started in the background with uiaccess to enable it to read the screen.  It seems like this might not be possible currently under MSIX without making the SnagIt capture runasadmin.


## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | June 2022 |


