# Packaging JT2Go for MSIX

The software was packaged on Windows 10 21H2 using Microsoft MSIX Packaging Tool 1.2022.512 with the PSF using TMEditX.
* PsfLauncher with  FileRedirectionFixup and either the DynamicLibrary fixup or LoaderSearchOrder to help find dlls. It also seems to need the RegLegacyFixup.


Testing on Windows 10/11 indicates  ![badge](https://img.shields.io/badge/-Major%20Issues-critical?style=for-the-badge) at this time. It is believed that the MSIX runtime has a bug in the containerized registry that is under investigation.  That the app has lots of VCRuntime components, both 120 and 140, may also contribute to app issues. 


## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | June 2022 |


