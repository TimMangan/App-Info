# Packaging JT2Go for MSIX

The app has been packaged in MSIX and requires the PSF FileRedirectionFixup and either the DynamicLibrary fixup or LoaderSearchOrder to help find dlls. It also seems to need the RegLegacyFixup.


Testing on Windows 10/11 indicates [<img src="/media/CatIssues.png" alt="Has Issues" />](/media/CatIssues.png) at this time. It is believed that the MSIX runtime has a bug in the containerized registry that is under investigation.  That the app has lots of VCRuntime components, both 120 and 140, may also contribute to app issues. 


## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | June 2022 |


