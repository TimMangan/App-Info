# Packaging CyberDuck for MSIX

The app has been packaged in MSIX without the PSF.
* If pre-configuration is needed, the PSF with FRF would be required.
* Modification of the AppXManifest to add ExecutionAlias is recommended:

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

Testing on Windows 10/11 indicates [<img src="/media/CatFullFidelity.png" alt="Full Fidelity" />](/media/CatFullFidelity.png).



## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | April 2022 |

