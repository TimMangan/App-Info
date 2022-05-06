# Packaging Password Depot for MSIX

The app has been packaged in MSIX with or without PSF.
* The PsfLauncher and FRF are needed (file based configuration in Program Files).
* It is necessary to keep shell extensions out of the package manifest due to duplicate guid issues.  It is unclear if these are really needed.


Testing on Windows 10/11 indicates [<img src="/media/CatHighConfidence.png" alt="High Confidence" />](/media/CatHighConfidence.png) due to missing Context menu.  
 


## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | April 2022 |


