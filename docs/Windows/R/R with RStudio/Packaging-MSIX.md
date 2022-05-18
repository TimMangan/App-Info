# Packaging R and RStudio for MSIX

The app has been packaged in MSIX with the PSF.  The PSfLauncher is needed, because there are both 32 and 64-bit exes with the same name that need a shortcut.  Due to file based configurations for the R launguage part of this package, the FRF is also needed.

The application attempts to install an FTA on .RData with a shell integration verb command using the same 'open' verb to start the 32 and 64 bit RGui.exe, one on .rdata and other on .RData.  MSIX cannot handle this and you must choose one or the other, but usually this means the 64 bit version.

The RStudio app uses a secondary process, `rsession.exe`, a 64-bit console application for which attempting to inject the PsfRuntime causes the app to fail.  Therefore the config.json file needs to not include a process block to inject the PSF.  As there are a large number of exe's in the package, it can be easier to add a process entry listing no injections for this exe, and having a default `.*` regex string to cover all other processes and add the FRF that way.

For some reason, `rsession.exe` fails to find the required dll files (like R.dll) from the R Language.  There are two copies of the R dlls, one for x86 and one for x64 and rsession needs the x64 ones.  Adding in a LoadSearchOrder entry into the AppXManifest file for the x64 R Language Dlls solves this issue.

## Packaging with MSIX Packaging Tool and fixing the package with TMEditX
One way to create a good package is to package using the Microsoft MSIX Packaging Tool and then fixing the package using TMEditX.  Other tooling could potentially also create a satisfactory package, but this is the technique known to work.  MMPT 2022.330 and TMEditX 2.3 were used in this documented success.

*  Package up using the Microsoft MSIX Packaging Tool.  Normal current best practices for using this tool are sufficient.
* Open the resulting package in TMEditX.
* * On the Analysis Page, first perform any package cleanup.
* * Then Add the PSF.
* * * In PsfLauncher, select the `Exclude Console Apps` option.
* * * Select the File Redirection Fixup with default options.
* * Back on the Analysis page, ignore the manifest fixup for FileTypeAssociation for .RData.
* * Select the fixup for the missing Fonts.
* * On the C.Files Tab, locate the R language folder for the x64 dlls for the version of R launguage, for example `VFS\ProgramFilesX64\R\R-4.1.0\bin\x64` and right-click to select the `Add folder to loaderSearhOrder` menu option.
* * Save the package.


Testing on Windows 10/11 indicates  [<img src="/media/CatFullFidelity.png" alt="Full Fidelity" />](/media/CatFullFidelity.png).  
 


## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | April 2022 |


