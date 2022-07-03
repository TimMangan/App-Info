# Packaging Dbeaver (Community Edition) for MSIX

The software was packaged on Windows 10 21H2 using Microsoft MSIX Packaging Tool 1.2022.330 without the PSF.

## WIP
Without the PSF we get an inability to load jvm.dll message.  However procmon trace shows it is loaded into memory OK,but then looks for VCRUNTIME140.dll which is not found.  It is in the package as vcruntime140.dll.

Dynamic library should help, but possibly a case issue?

LSO on the folder for jre/bin solves it.  Still don't know what causes native install to find this...


Testing on Windows 10/11 indicates ![badge](https://img.shields.io/badge/-Full%20Fidelity-brightgreen?style=for-the-badge).



## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | May 2022 |

