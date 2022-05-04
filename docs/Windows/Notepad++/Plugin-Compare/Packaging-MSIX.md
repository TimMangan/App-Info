# Packaging Notepad++ Plugin for MSIX

The app has been packaged in MSIX.  
* Adding the PSF to this package is not appropriate as it does not have any entry points.
* Unlike the App-V Sequencer, there is no "expand package" functionality built into the Microsoft MSIX Packageing Tool (MMPT), so you must install NotePad++ on the packaging system priot to starting the packaging process (install the same way it was installed in your NotepadPlusPlus package).
* Do one of the following:
* * In the MMPT, select the Modification Package option, and select your NotePadPlusPlus package so that this modification package will link to the primary package (eliminating the need for creating a connection group). At the client this imposes an installation order (main app prior to plugin) and the plugin appears as an addon to the main app rather than a separate app.
* * In the MMPT, select the New Application Package. You don't reference the main package. At the client, installs may be installed in any order, but you'll need to add a "Shared Package Container" to bring the apps together (Requires Windows 11).


Testing on Windows 10/11 indicates [<img src="/media/CatFullFidelity.png" alt="Full Fidelity" />](/media/CatFullFidelity.png) by using the Modification method.  


## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | April 2022 |


