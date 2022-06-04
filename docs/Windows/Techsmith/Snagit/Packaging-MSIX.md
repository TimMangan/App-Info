# Packaging SnagIt for MSIX

The app has been packaged in MSIX with the PSF and FileRedirectionFixup.
* FileRedirectionFixup might be needed to enable writing to a wide variety of ini and xml files.
* TMEditX was used for the following fixups to the package produced by the MSIX Packaging Tool:
* * Context Menus (you may choose to fix either "*" or "Directory" but not both due to AppXManifest limitations).
* * Image Handler.
* * Missing Fonts.
* * ExecutionAlias for Snagit32.exe.



Testing on Windows 10/11 indicates  [<img src="/media/CatIssues.png" alt="Has Issues" />](/media/CatIssues.png).  The application includes a component, SnagPriv.exe, that is started in the background with uiaccess to enable it to read the screen.  It seems like this might not be possible currently under MSIX without making the SnagIt capture runasadmin.


## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | June 2022 |


