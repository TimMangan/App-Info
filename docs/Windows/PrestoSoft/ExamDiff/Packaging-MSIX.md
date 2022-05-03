# Packaging ExamDiff for MSIX

The app has been packaged in MSIX with or without PSF.
* PsfLauncher is required if shortcuts to the read me or what's new are left in the package.
* There is an issue with being able to set and save some registry configuration.  This is something that RegLegacyFixup cannot fix.  It is possible to overcome this limitation by including all configuration options in the package originally, which will allow the end-user to modify them.  As the options are very important in this app, you can probably live without them.


Testing on Windows 10/11 indicates [<img src="/media/CatFullFidelity.png" alt="Full Fidelity" />](/media/CatFullFidelity.png).  
