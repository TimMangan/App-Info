# Packaging Notepad++ for MSIX

The software was packaged on Windows 10 21H2 using Microsoft MSIX Packaging Tool 1.2022.330 and edited in TMEditX with PSF, DynanicDll and EnvVar fixups.
* The PsfLauncher and FRF are needed, possibly for file based xml files in Program Files, but if preconfiguration in AppData\Roaming is used.
* The Package Name may not include the '+' charactor, so many people replace this with the word 'Plus'.
* If you plan to have plugin packages using the Modification Package method, this package must be installed using VFS pathing.


Testing on Windows 10 indicates ![badge](https://img.shields.io/badge/-High%20Confidence-green?style=for-the-badge).  The issue preventing full fidelity is that the support for the type of Shell Extension Context Menu is only supported in MSIX packages on Windows 11.

Testing on Windows 11 indicates ![badge](https://img.shields.io/badge/-Full%20Fidelity-brightgreen?style=for-the-badge).  


## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | April 2022 |


