# Packaging Audacity for MSIX

The software was packaged on Windows 10 21H2 using Microsoft MSIX Packaging Tool 1.2022.330 and enhanced by editing with TMEditX to inject the PSF.
* The Launcher and FRF are needed due to files in AppData.


Testing on Windows 10 indicates ![badge](https://img.shields.io/badge/-Major%20Issues-critical?style=for-the-badge) support of the app.
* The app complains about the cfg file, althogh we see it being read. The app will only close.  This app used to work in MSIX, so we suspect this may be the well known registry bug.



## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | April 2022 |


