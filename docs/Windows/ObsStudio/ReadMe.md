# App-Info Document OBS Studio

<div>

<img src="/media/AppIcons/OBSSixFour-256.png" align="left" height="256" alt="ObsStudio logo"  /> ObsStudio ia a popular free and open source software for video recording and especially live streaming.

This Readme.md is the high level file that describes the application summary.  Additional documentation files may also be present to cover specific scenarios, such as repackaging into a specific format. See the file list in this folder.
 
</div>
<p> </p>

## Documentation for

| Category | Value |
|-----|-------------------------------------------------------|
| Vendor Name | ObsProject.org |
| Application Name| OBS Studio |
| Application Version | 27.0.1 (released 2021/08, newer version available) |
| Vendor/App Website| https://obsproject.com |



## Vendor Installer Types

This is where we can define the forms of installers available from the vendor. 
<table >
<tr>
<td>

| Installer Type Availabilty |
|----|
| ![badge](https://img.shields.io/badge/Zip-Yes-green?style=for-the-badge)  See `Note1`|
| ![badge](https://img.shields.io/badge/Setup%20Exe-Yes-green?style=for-the-badge) |
| ![badge](https://img.shields.io/badge/MSI-No-red?style=for-the-badge) |
| ![badge](https://img.shields.io/badge/AppX%2FBundle-No-red?style=for-the-badge) |
| ![badge](https://img.shields.io/badge/MSIX%2FBundle-No-red?style=for-the-badge) |
| ![badge](https://img.shields.io/badge/appinstaller-No-red?style=for-the-badge) |

</td>
<td width=100></td>
<td>

| Code Architecture Availabilty |
|----|
| ![badge](https://img.shields.io/badge/x86-Yes-green?style=for-the-badge) |
| ![badge](https://img.shields.io/badge/x64-Yes-green?style=for-the-badge) |
| ![badge](https://img.shields.io/badge/AnyCPU-No-red?style=for-the-badge) |
| ![badge](https://img.shields.io/badge/Arm-No-red?style=for-the-badge) |
| ![badge](https://img.shields.io/badge/Arm64-No-red?style=for-the-badge) |

</td>
</tr>
</table>


`Note1`: Zip contains loose files of the x64 without installer.

## App Configuration Type

This is where to place a summary of how application configuration is stored.  Items of configuration of common interest should be documented in a separate file. See [InstallConfigure](InstallConfigure.md) for more information.

| Configuration Style Availability |
|----
| ![badge](https://img.shields.io/badge/Registry-No-red?style=for-the-badge) |
| ![badge](https://img.shields.io/badge/File-Yes-green?style=for-the-badge) |
| ![badge](https://img.shields.io/badge/AD%2FGPO-No-red?style=for-the-badge) |
| ![badge](https://img.shields.io/badge/AAD%2FGPO-No-red?style=for-the-badge) |


## Repackaging Summary

This is where to list a summary of known success (or not) in repackaging info certain formats.  If repackaging the application is not straightforward, a specific documentation file covering the details for that repackaging format is suggested. Values in the Success field are somewhat subjective, but we recommend that the summary use the following value:

* ![badge](https://img.shields.io/badge/-Full%20Fidelity-brightgreen?style=for-the-badge) - App appears to be completely functional.
* ![badge](https://img.shields.io/badge/-High%20Confidence-green?style=for-the-badge) - There may be a small loss in functionality, but most companies will be OK with deploying this form.
* ![badge](https://img.shields.io/badge/-Mostly%20Works-yellow?style=for-the-badge) - A loss in functionality that likely makes this a bad way to deploy.
* ![badge](https://img.shields.io/badge/-Major%20Issues-critical?style=for-the-badge) - Application is known to not work in this form (so far).
* ![badge](https://img.shields.io/badge/-Unknown%2FUntested-lightgray?style=for-the-badge) - No information is available.

See [Testing](Testing.md) for details on the testing performed on this app.

| Repackaging type | Tested result |
|----|----|
| MSI | ![badge](https://img.shields.io/badge/-Unknown%2FUntested-lightgray?style=for-the-badge) |
| [App-V](Packaging-AppV.md) | ![badge](https://img.shields.io/badge/-Full%20Fidelity-brightgreen?style=for-the-badge) |
| ThinApp | ![badge](https://img.shields.io/badge/-Unknown%2FUntested-lightgray?style=for-the-badge) |
| Citrix App Layers | ![badge](https://img.shields.io/badge/-Unknown%2FUntested-lightgray?style=for-the-badge) |
| Cloud Volumes | ![badge](https://img.shields.io/badge/-Unknown%2FUntested-lightgray?style=for-the-badge) |
| FlexApp | ![badge](https://img.shields.io/badge/-Unknown%2FUntested-lightgray?style=for-the-badge) |
| Numecent | ![badge](https://img.shields.io/badge/-Unknown%2FUntested-lightgray?style=for-the-badge) |
| [MSIX](Packaging-MSIX.md) | ![badge](https://img.shields.io/badge/-Full%20Fidelity-brightgreen?style=for-the-badge) |

## Useful links
This is a place to put useful links to appropriate existing external sources, either those of the vendor or elsewhere.
