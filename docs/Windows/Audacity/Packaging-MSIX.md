# Packaging Audacity for MSIX

The app has been packaged in MSIX:
* The Launcher and FRF are needed.

* The shortcut to the .chm file may be ignored by some packaging tools. This is usually OK, but the PSF PsfLauncher may be used to make this available. 

Testing on Windows 10 indicates [<img src="/media/CatIssues.png" alt="Has Issues" />](/media/CatIssues.png) support of the app.
* The app complains about the cfg file, althogh we see it being read. The app will only close.
