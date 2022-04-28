# Packaging Anaconda for MSIX

The app has been packaged in MSIX with the PSF.
* The [{Personal}] folder exclusion should be removed before repackaging.
* PsfLauncher is required as is the FRF.

Testing on Windows 10/11 indicates [<img src="/media/CatIssues.png" alt="Has Issues" />](/media/CatIssues.png).  These issues were from the use of the Microsoft MSIX Packaging Tool; perhaps other tooling will work.
