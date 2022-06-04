# Packaging Camtasia for MSIX

The app has been packaged in MSIX without the PSF.
* FileRedirectionFixup might be needed to enable writing to a wide variety of ini and xml files, but see next issue.
* EdgeWebView2 does not work from inside the package.  Deployint this externally to clients did not work either.  

NOTE: Earlier versions of Camtasia did not include WebView2 requirement and worked great under MSIX.



Testing on Windows 10/11 indicates  [<img src="/media/CatIssues.png" alt="Has Issues" />](/media/CatIssues.png).


## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | June 2022 |


