# Packaging ActivePython for MSIX

The app has been packaged in MSIX with the PSF.

* PsfLauncher is required for some of the shortcuts.
* The FRF is needed for the developer to configure their environment.

Testing on Windows 10/11 indicates [<img src="/media/CatIssues.png" alt="Has Issues" />](/media/CatIssues.png) that make this application a bad candidate at this time.  

* The issues seem to come from the Microsoft MSIX Packaging Tool, so perhaps repackaging using a different vendor might help.
* It might be necessary to force the install to Program Files, however this was not attempted.


## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | April 2022 |

