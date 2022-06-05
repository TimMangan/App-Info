# Packaging AdobeReader DC for MSIX

The app has been packaged in MSIX with the PSF.

The software was packaged on Windows 10 21H2 using Microsoft MSIX Packaging Tool 1.2022.330 and enhanced by editing with TMEditX to inject the PSF.
* PsfLauncher is required as is the FRF.

Testing on Windows 10/11 indicates ![badge](https://img.shields.io/badge/-Mostly%20Works-yellow?style=for-the-badge), and any company considering MSIX deployment should througly test the package.  

* Internet Explorer integration is not possible with MSIX.  When this is not an issue at your company, the validation is raised to ![badge](https://img.shields.io/badge/-High%20Confidence-green?style=for-the-badge).
* The other most noticable issue is that the License Agreement popup appears.



## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | April 2022 |

