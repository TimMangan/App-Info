# Packaging MikTex for MSIX

The software was packaged on Windows 10 21H2 using Microsoft MSIX Packaging Tool 1.2022.512 both with and without the PSF using TMEditX 2.4.
* The `MiKTex Console` shortcut and the respository folder were removed after installation.
* The PSF Launcher, and FRF fixups are used as suggested; DynnamicDll and RegLegacyFixup should also be added using default settings.
* The Microsoft MSIX Packaging tool ignores the considerable number of fonts that are an important part of this package.  TMEditX takes care of this easily, but otherwise a manual edit to the AppXManifest file would be needed.


Testing on Windows 10/11 indicates ![badge](https://img.shields.io/badge/-Full%20Fidelity-brightgreen?style=for-the-badge), however additional debugging is warrented.  


## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | July 2022 |


