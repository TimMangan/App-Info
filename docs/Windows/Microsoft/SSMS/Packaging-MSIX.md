# Packaging SSMS for MSIX

The app has been packaged in MSIX both with and without the PSF.
* The PSF Launcher, FRF, and EnvVarFixups are recommended.
* The launch of the primary app fails; possibly it still uses unsupported COM+.


Testing on Windows 10/11 indicates [<img src="/media/CatIssues.png" alt="Has Issues" />](/media/CatIssues.png).  

There is a blog post claiming that a MSIX package can work by manually turning off part of the container virtual registry, in essence using pass through keys.  I did not verify that this solves all problems with the package, but looks promising until Microsoft solves the container registry issue that we are seeing on a number of apps.  See https://techcommunity.microsoft.com/t5/windows-dev-appconsult/azure-virtual-desktop-avd-packaging-the-sql-server-management/ba-p/3457856 

## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | April 2022 |


