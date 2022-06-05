# Packaging Thunderbird for MSIX


The software was packaged on Windows 10 21H2 using Microsoft MSIX Packaging Tool 1.2022.330 both with and without the PSF.
* During the install, the maintenance service was disabled.  It may be advantagious to remove this unnecessary service while in monitoring mode.  Otherwise, the AppXManifest will be marked for the service capability and elevation is needed when manual installation of this package is performed by a standard user (but typically not an issue for software deployment tools)
* Although the package has some ini files, these are not routinely changed during production use of the software, so the FRF may not be not needed, however it was used our packaging just in case.
* When the PSF was included, PsfLauncher is required as is the  EnvVar fixup; FRF is also recommended.
* Testing without the PSF also passed the 'smoke test', but we are more comfortable with the PSF in the package for production use on this app.


Testing on Windows 10/11 indicates ![badge](https://img.shields.io/badge/-Full%20Fidelity-brightgreen?style=for-the-badge).  


## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | April 2022 |


