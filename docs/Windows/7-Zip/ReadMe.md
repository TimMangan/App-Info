# App-Info Document 7-Zip

<div>

<img src="/media/AppIcons/SevenZFM-256.png" align="left" valign="top" height="256" alt="7-Zip logo"  /> 7-zip is a freeware version of an archive (aka "Zip") compression/decompression tool issued via GNU license. It also has open-source code available.  

<p> </p>

This software is popular among IT Pros because it also includes the ability to extract files from inside of WinPE files.  For example, such as to access embedded MSI from the setup.exe installers.  Ot so extract icons and other resources from an exe or dll file.

<p> </p>

 7-Zip does have its own format and file-type (.7z), but works with standard zip and rar compressed archives.
 
<p> </p>

This Readme.md is the high level file that describes the application summary.  Additional documentation files may also be present to cover specific scenarios, such as repackaging into a specific format. See the file list in this folder.
 
</div>

<p> </p>


## Documentation for

| Category | Value |
|-----|-------------------------------------------------------|
| Vendor Name | 7-Zip (Igor Pavlov) |
| Application Name| 7-Zip |
| Application Version | 19.00 (released 2019/02, newer versions available)|
| Vendor/App Website| www.7-zip.org |



## Vendor Installer Types

This is where we can define the forms of installers available from the vendor.
<table >
<tr>
<td>

| Installer Type Availabilty |
|----|
| ![badge](https://img.shields.io/badge/Setup%20Exe-Yes-green?style=for-the-badge) |
| ![badge](https://img.shields.io/badge/MSI-Yes-green?style=for-the-badge) |
| ![badge](https://img.shields.io/badge/AppX%2FBundle-No-red?style=for-the-badge) |
| ![badge](https://img.shields.io/badge/MSIX%2FBundle-No-red-lightgrey?style=for-the-badge) |
| ![badge](https://img.shields.io/badge/appinstaller-No-red-lightgrey?style=for-the-badge) |

</td>
<td width=100></td>
<td>

| Code Architecture Availabilty |
|----|
| ![badge](https://img.shields.io/badge/x86-Yes-green?style=for-the-badge) |
| ![badge](https://img.shields.io/badge/x64-Yes-green?style=for-the-badge) |
| ![badge](https://img.shields.io/badge/AnyCPU-Unknown-lightgrey?style=for-the-badge) |
| ![badge](https://img.shields.io/badge/Arm-No-red?style=for-the-badge) |
| ![badge](https://img.shields.io/badge/Arm64-Yes-green?style=for-the-badge) |


</td>
</tr>
</table>

## App Configuration Type

This is where to place a summary of how application configuration is stored.  Items of configuration of common interest should be documented in a separate file.

| Configuration Style Availability |
|----
| ![badge](https://img.shields.io/badge/Registry-Yes-green?style=for-the-badge) |
| ![badge](https://img.shields.io/badge/File-No-red?style=for-the-badge) |
| ![badge](https://img.shields.io/badge/AD%2FGPO-No-red?style=for-the-badge) |
| ![badge](https://img.shields.io/badge/AAD%2FGPO-No-red?style=for-the-badge) |


## Repackaging Summary

This is where to list a summary of known success (or not) in repackaging info certain formats.  If repackaging the application is not straightforward, a specific documentation file covering the details for that repackaging format is suggested. Values in the Success field are somewhat subjective, but we recommend that the summary use the following value:

* ![badge](https://img.shields.io/badge/-Full%20Fidelity-brightgreen?style=for-the-badge) - App appears to be completely functional.
* ![badge](https://img.shields.io/badge/-High%20Confidence-green?style=for-the-badge) - There may be a small loss in functionality, but most companies will be OK with deploying this form.
* ![badge](https://img.shields.io/badge/-Mostly%20Works-yellow?style=for-the-badge) - A loss in functionality that likely makes this a bad way to deploy.
* ![badge](https://img.shields.io/badge/-Major%20Issues-critical?style=for-the-badge) - Application is known to not work in this form (so far).
* ![badge](https://img.shields.io/badge/-Unknown%2FUntested-lightgray?style=for-the-badge) - No information is available.


| Repackaging type | Tested result |
|----|----|
| MSI | ![badge](https://img.shields.io/badge/-Unknown%2FUntested-lightgray?style=for-the-badge) |
| [App-V](Packaging-AppV.md) | ![badge](https://img.shields.io/badge/-Full%20Fidelity-brightgreen?style=for-the-badge) |
| ThinApp | ![badge](https://img.shields.io/badge/-Unknown%2FUntested-lightgray?style=for-the-badge) |
| Citrix App Layers | ![badge](https://img.shields.io/badge/-Unknown%2FUntested-lightgray?style=for-the-badge) |
| Cloud Volumes | ![badge](https://img.shields.io/badge/-Unknown%2FUntested-lightgray?style=for-the-badge) |
| FlexApp | ![badge](https://img.shields.io/badge/-Unknown%2FUntested-lightgray?style=for-the-badge) |
| Numecent | ![badge](https://img.shields.io/badge/-Unknown%2FUntested-lightgray?style=for-the-badge) |
| [MSIX](Packaging-MSIX.md) | ![badge](https://img.shields.io/badge/-High%20Confidence-green?style=for-the-badge) on Windows 10 ![badge](https://img.shields.io/badge/-Full%20Fidelity-brightgreen?style=for-the-badge) on Windows 11 |

## Useful links
This is a place to put useful links to appropriate existing external sources, either those of the vendor or elsewhere.
