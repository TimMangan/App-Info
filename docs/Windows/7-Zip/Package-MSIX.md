# Packaging 7-Zip for MSIX

The app is easily packaged in MSIX and requires little special treatment:

* The shortcut to the .chm file may be ignored by some packaging tools. This is usually OK, but the PSF PsfLauncher may be used to make this available. 

Testing on Windows 10 indicates [<img src="/media/CatHighConfidence.png" alt="High Confidence" />](/media/CatHighConfidence.png) support of the app.
* Some of the Shell Extensions are not available. 

Testing on Windows 11 indicates [<img src="/media/CatFullFidelity.png" alt="Full Fidelity" />](/media/CatFullFidelity.png) support of the app.
* The shell extensions are available thanks to the Desktop9 schema extensions.