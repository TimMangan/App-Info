# Packaging Gimp for MSIX

The software was packaged on Windows 10 21H2 using Microsoft MSIX Packaging Tool 1.2022.330 and enhanced by editing with TMEditX to inject the PSF.
* After install, copy configuration file with desired settings under `Program Files\Gimp 2`..
* PsfLauncher is required as is the FRF.
* It is also neccessary to add a package level extension to the AppXManifest for two directories for loadsearchpathorder as shown below:

```xml
<Package>
    ...
    <Applications>
        ...
    </Applications>
    <Extensions>
        <uap6:Extension Category="windows.loaderSearchPathOverride">
            <uap6:LoaderSearchPathOverride>
                <uap6:LoaderSearchPathEntry FolderPath="VFS\ProgramFilesX64\GIMP 2\32\bin"/>
                <uap6:LoaderSearchPathEntry FolderPath="VFS\ProgramFilesX64\GIMP 2\bin"/>
            </uap6:LoaderSearchPathOverride>
        </uap6:Extension>
    </Extensions>
    ...
</Package>
```


Testing on Windows 10/11 indicates ![badge](https://img.shields.io/badge/-Full%20Fidelity-brightgreen?style=for-the-badge).  


## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | April 2022 |


