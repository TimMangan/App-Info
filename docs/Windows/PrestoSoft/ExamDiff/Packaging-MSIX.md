# Packaging ExamDiff for MSIX

The software was packaged on Windows 10 21H2 using Microsoft MSIX Packaging Tool 1.2022.330 with or without PSF using TMEditX.
* PsfLauncher is required if shortcuts to the read me or what's new are left in the package.
* There is an issue with being able to set and save some registry configuration.  This is something that RegLegacyFixup cannot fix.  It is possible to overcome this limitation by including all configuration options in the package originally, which will allow the end-user to modify them.  As the options are very important in this app, you can probably live without them.


Testing on Windows 10/11 indicates ![badge](https://img.shields.io/badge/-Full%20Fidelity-brightgreen?style=for-the-badge).  


## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | April 2022 |


