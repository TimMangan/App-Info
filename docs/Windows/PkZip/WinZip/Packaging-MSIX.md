# Packaging WinZip for MSIX

The software was packaged on Windows 10 21H2 using Microsoft MSIX Packaging Tool 1.2022.330 with the PSF using TMEditX 2.3.  In TMEditX, the following changes were needed:
* PsfLauncher with FileRedirectionFixup need to be added.
* Missing Preview Handlers should not be fixed at this time because the same Com dll is used for different types and the Manifest does not yet support this.
* Manifest has no support for the DropHandlers yet.
* Missing Shell integration verbs for 'print' can be fixed if needed.
* Missing Protocol Handler should be fixed.
* Missing ExecutionAlias entries should be fixed.
* Missing LoaderSearchOrder entry should be fixed.


Testing on Windows 10/11 indicates  ![badge](https://img.shields.io/badge/-Mostly%20Works-yellow?style=for-the-badge) due to:
* App elevates on launch.  Unknown cause.
* Missing Context menu, even on Windows 11.
* Dropping a file/folder on a zip file once you make WinZip the default for .zip files doesn't add to zip file but acts as a copy/move to the folder that the zip file is in.
 


## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | June 2022 |


