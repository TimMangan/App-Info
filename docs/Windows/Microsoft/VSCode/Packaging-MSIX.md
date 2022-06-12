# Packaging VSCode for MSIX

The software was packaged on Windows 10 21H2 using Microsoft MSIX Packaging Tool 1.2022.512 both with the PSF using TMEditX.
* The PSF Launcher, with FRF are recommended.
* TMEditX is also used to add the 2 fonts to the manifest..


Testing on Windows 10/11 indicates ![badge](https://img.shields.io/badge/-Major%20Issues-critical?style=for-the-badge) .  

While the basic product is fine, Extensions are having an issue. So while it would be possible to build a package with the extensions already in there, it just isn't a reasonable way to deploy.  While the FRF should help, the issue is how the app tries to do file work in two different parts, leading to different redirection paths generated.

## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | April 2022 |


