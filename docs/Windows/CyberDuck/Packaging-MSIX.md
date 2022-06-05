# Packaging CyberDuck for MSIX

The software was packaged on Windows 10 21H2 using Microsoft MSIX Packaging Tool 1.2022.330 without the PSF.
* If pre-configuration is needed, the PSF with FRF would be required.
* Modification of the AppXManifest to add ExecutionAlias is recommended. This may be done manually in the manifest editor of the MMPT or button-click in TMEditX:

``` xml
<Package ...>
    ...
    <Applications>
        <Application ...>
            ...
            <Extensions>
                ...
                <uap3:Extension category="windows.appExecutionAlias">
                    <uap3:AppExecutionAlias>
                        <desktop:ExecutionAlias Alias="CyberDuck.exe">
                    </uap3:AppExecutionAlias>
                </uap3:Extension>
            </Extensions>
        </Application>
        ...
    </Applications>
    ...
</Package>
```

Testing on Windows 10/11 indicates ![badge](https://img.shields.io/badge/-Full%20Fidelity-brightgreen?style=for-the-badge).



## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | April 2022 |

