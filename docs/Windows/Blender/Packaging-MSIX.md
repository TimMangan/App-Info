# Packaging Blender for MSIX

## Blender 3.0
The software was packaged on Windows 10 21H2 using Microsoft MSIX Packaging Tool 1.2022.330 and enhanced by editing with TMEditX to inject the PSF.
* PsfLauncher is required as is the FRF.

Testing on Windows 10/11 indicates ![badge](https://img.shields.io/badge/-Full%20Fidelity-brightgreen?style=for-the-badge). 

## Blender 3.3.1 LTS
The software was packaged on Windows 10 21H2 using Microsoft MSIX Packaging Tool 1.2022.1101 and enhanced by editing with TMEditX to add InstallationLocationVirtualization support.

This version from the vendor placed two font files in an incorrect folder, which coincendentally works for the native installation, but under MSIX fails without modification.  These two fonts are found a few folders under `C:\Program Files\BlenderFoundation` (note the lack of space whereas `C:\Program Files\Blender Foundation` is where the program installs.

After installing, it is necessary to copy the two ttf files from the path without the space to the path with the space.

The package was creating by adding the InstalledLocationVirtualization feature instead of the PSF.  This seems to work for now.  There is concern that we might need to swap out the shortcut, which now points to blender-launcher, to that of the main program blender.  It is likely that the launcher is looking for updates (which will probably not happen on the LTS until next August) and we should bypass this component, but we are not yet sure all that it does.


Testing on Windows 10/11 indicates ![badge](https://img.shields.io/badge/-Full%20Fidelity-brightgreen?style=for-the-badge). 


## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | April 2022 | [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | December 2022 |


