# Packaging Power BI Desktop for MSIX

The software was packaged on Windows 10 21H2 using Microsoft MSIX Packaging Tool 1.2022.512 without the PSF.  Adding the PSF to this app causes a CLR issue, so best to avoid. 


Testing on Windows 10/11 indicates ![badge](https://img.shields.io/badge/-High%20Confidence-green?style=for-the-badge).  This rating is given when the app is deployed without a license.  An error dialog appears on the first run, but appears to be benign and does not reappear. Since this is an app used by power users that seems OK to ignore. 


## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | April 2022 |


