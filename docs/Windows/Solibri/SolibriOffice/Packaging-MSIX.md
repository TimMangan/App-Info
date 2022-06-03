# Packaging Solibri Office for MSIX

The app has been packaged in MSIX with the PSF FileRedirection Fixup and DynamicLibraryFixup.
* TMEditX was used to add FONTS into the AppXManifest.



Testing on Windows 10/11 indicates [<img src="/media/CatIssues.png" alt="Has Issues" />](/media/CatIssues.png).

The app includes a copy of a Java JRE, however it isn't being found by the app when launched in the container.  This needs more investigation, but seems like it is the known runtime issue with the registry. 


## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | June 2022 |


