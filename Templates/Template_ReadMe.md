# App-Info Document Template (replace this with your application name)



Please remove the boiler plate at and above this line, then edit the example below.
_____

<div>

<img src="/media/AppIcons/App-Info.png" align="left" height="256" alt="XXX logo"  />  Swap an icon for the app to the left. This application is used for some purpose. I like to include information on if it is free or a licensed app.  And if there is open source available, if I know about it.

Maybe some more text as you want enough to get the 256 bit icons to be covered before the documentation header below.  This can mean about 10 lines of text.

This Readme.md is the high level file that describes the application summary.  Additional documentation files may also be present to cover specific scenarios, such as repackaging into a specific format. See the file list in this folder. 

</div>
<p> </p>

## Documentation for

| Category | Value |
|-----|-------------------------------------------------------|
| Vendor Name | XXX |
| Application Name| XXX |
| Application Version | XXX Leave blank if version specific doc files exist. |
| Vendor/App Website| XXX |



## Vendor Installer Types

This is where we can define the forms of installers available from the vendor.
<table >
<tr>
<td>

| Installer Type Availabilty |
|----|
| ![badge](https://img.shields.io/badge/Setup%20Exe-No-red?style=for-the-badge) |
| ![badge](https://img.shields.io/badge/MSI-Yes-green?style=for-the-badge) |
| ![badge](https://img.shields.io/badge/AppX%2FBundle-Unknown-lightgrey?style=for-the-badge) |
| ![badge](https://img.shields.io/badge/MSIX%2FBundle-Unknown-lightgrey?style=for-the-badge) |
| ![badge](https://img.shields.io/badge/appinstaller-Unknown-lightgrey?style=for-the-badge) |

</td>
<td width=100></td>
<td>

| Code Architecture Availabilty |
|----|
| ![badge](https://img.shields.io/badge/x86-No-red?style=for-the-badge) |
| ![badge](https://img.shields.io/badge/x64-Yes-green?style=for-the-badge) |
| ![badge](https://img.shields.io/badge/AnyCPU-No-red?style=for-the-badge) |
| ![badge](https://img.shields.io/badge/Arm-No-red?style=for-the-badge) |
| ![badge](https://img.shields.io/badge/Arm64-Unknown-lightgrey?style=for-the-badge) |

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
| ![badge](https://img.shields.io/badge/AAD%2FGPO-Unknown-lightgrey?style=for-the-badge) |

## Repackaging Summary

This is where to list a summary of known success (or not) in repackaging info certain formats.  If repackaging the application is not straightforward, a specific documentation file covering the details for that repackaging format is suggested. Values in the Success field are somewhat subjective, but we recommend that the summary use the following value:

* ![badge](https://img.shields.io/badge/-Full%20Fidelity-brightgreen?style=for-the-badge) - App appears to be completely functional.
* ![badge](https://img.shields.io/badge/-High%20Confidence-green?style=for-the-badge) - There may be a small loss in functionality, but most companies will be OK with deploying this form.
* ![badge](https://img.shields.io/badge/-Mostly%20Works-yellow?style=for-the-badge) - A loss in functionality that likely makes this a bad way to deploy.
* ![badge](https://img.shields.io/badge/-Major%20Issues-critical?style=for-the-badge) - Application is known to not work in this form (so far).
* ![badge](https://img.shields.io/badge/-Work%20In%20Progress-blue?style=for-the-badge) - Work in progress.
* ![badge](https://img.shields.io/badge/-Unknown%2FUntested-lightgray?style=for-the-badge) - No information is available.


| Repackaging type | Tested result |
|----|----|
| MSI | ![badge](https://img.shields.io/badge/-Unknown%2FUntested-lightgray?style=for-the-badge) |
| App-V | ![badge](https://img.shields.io/badge/-Full%20Fidelity-brightgreen?style=for-the-badge) |
| ThinApp | ![badge](https://img.shields.io/badge/-Unknown%2FUntested-lightgray?style=for-the-badge) |
| Citrix App Layers | ![badge](https://img.shields.io/badge/-Unknown%2FUntested-lightgray?style=for-the-badge) |
| Cloud Volumes | ![badge](https://img.shields.io/badge/-Unknown%2FUntested-lightgray?style=for-the-badge) |
| FlexApp | ![badge](https://img.shields.io/badge/-Unknown%2FUntested-lightgray?style=for-the-badge) |
| Numecent | ![badge](https://img.shields.io/badge/-Unknown%2FUntested-lightgray?style=for-the-badge) |
| MSIX | ![badge](https://img.shields.io/badge/-Unknown%2FUntested-lightgray?style=for-the-badge) |

## Useful links
This is a place to put useful links to appropriate existing external sources, either those of the vendor or elsewhere.
