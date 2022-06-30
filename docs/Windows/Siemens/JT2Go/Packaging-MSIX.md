# Packaging JT2Go for MSIX

The software was packaged on Windows 10 21H2 using Microsoft MSIX Packaging Tool 1.2022.512 with the PSF using TMEditX.
* Installation was done using typical edits of the cmd file provided by the vendor.
* Additionally, due to a current bug in the containerized registry, it is necessary to pre-create the registry `HKCU\Software\JT2Go_Retained\13.3\Common\C\VPSearch\LocationCache` (for version 13.2.xxx) to avoid a runtime issue involving this key.
* It is possible to pre-authorize the license agreement via registry as well.
* PsfLauncher with  FileRedirectionFixup.  It also seems to migrate the external manifest file "Registration-free COM" private registration into the AppXManifest file (TMEditX 2.4 and above support automating this migration).


Testing on Windows 10/11 indicates  ![badge](https://img.shields.io/badge/-Full%20Fidelity-brightgreen?style=for-the-badge) at this time.


## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | June 2022 |


