# Packaging for MSIX

The app is easily packaged in MSIX and requires little special treatment:

* The shortcut to the .chm file may be ignored by some packaging tools. This is usually OK, but the Psf PsfLauncher may be used to make this available. 

Testing on Windows 10 indicates `High Confidence` support of the app.
* Some of the Shell Extensions are not available. 

Testing on Windows 11 indicates `Full-Fidelity` support of the app.
* The shell extensions are available thanks to the Desktop9 schema extensions.