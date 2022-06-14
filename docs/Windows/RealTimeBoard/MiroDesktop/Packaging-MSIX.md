# Packaging Mira Desktop for MSIX

The app has been packaged in MSIX using the Microsoft MSIX Packaging Tool 1.2022.512 with using TMEditX to inject the PSF.  The Launcher and FileRedirectionFixup are required.

The MSI version of the installer (without updates) was used.
* The MSI version supports silent ('/q') and passive ('/passive') options.  No other parameters of significance were found.
* After the MSI is installed, the command placed in the Run key must be executed. This is ` "C:\Program Files\Miro Installer\RealtimeBoard.exe" --checkInstall `.
* That command will run in the background.  It is necessary to wait for it to complete. If using an installation script, a sleep for 3 minutes should be sufficient.


Testing on Windows 10/11 indicates [MSIX](Packaging-MSIX.md) | ![badge](https://img.shields.io/badge/-Work%20In%20Progress-blue?style=for-the-badge) support of the app, with the following notes:

* First launch of the app by the user was slow.  Subsequent launches seem fine.
* No account was available to test, so UAT testing is really needed to confirm this result.



## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | May 2022 |

