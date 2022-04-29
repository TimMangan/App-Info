# Packaging Fiddler for MSIX

The app has been packaged in MSIX with the PSF.
* After install, import reg file with desired settings.
* Remove the uninst.exe from the program folder.
* While monitoring, run 'EnableLoopback.exe -All'
* PsfLauncher is required as is the RegLegacy, and EnvVar fixups.


Testing on Windows 10/11 indicates [<img src="/media/CatHighConfidence.png" alt="High Confidence" />](/media/CatHighConfidence.png).  
