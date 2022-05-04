# Packaging Notepad++ for MSIX

The app has been packaged in MSIX with PSF, DynanicDll and EnvVar fixups.
* The PsfLauncher and FRF are needed, possibly for file based xml files in Program Files, but if preconfiguration in AppData\Roaming is used.
* The Package Name may not include the '+' charactor, so many people replace this with the word 'Plus'.
* If you plan to have plugin packages using the Modification Package method, this package must be installed using VFS pathing.


Testing on Windows 10 indicates [<img src="/media/CatHighConfidence.png" alt="High Confidence" />](/media/CatHighConfidence.png).  The issue preventing full fidelity is that the support for the type of Shell Extension Context Menu is only supported in MSIX packages on Windows 11.

Testing on Windows 11 indicates [<img src="/media/CatFullFidelity.png" alt="Full Fidelity" />](/media/CatFullFidelity.png).  


## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | April 2022 |


