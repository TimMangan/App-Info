# App-Info Document DosBox_Blockout

<div>

<img src="/media/AppIcons/DOSBOX-256.png" align="left" height="100" alt="DosBox logo"  /> This package is an example of a 16-bit DOS application, which natively could no longer run on x64 systems.  We include DosBox as a way to host this app; packaging them together and using DosBox as the shortcut that automatically launches the 16-bit app in its emulator.

The specific 16-bit app in this package is Blockout, a Tetris like game, but the concept here holds for a bunch of old 16-bit business apps that are still in use today, mostly by Small companies.  Often, these 16-bit apps are an ancient line of business app that they just can't live without and will continue to use until the owner of the business retires or passes away.

This Readme.md is the high level file that describes the application summary.  Additional documentation files may also be present to cover specific scenarios, such as repackaging into a specific format. See the file list in this folder.
 
</div>
<p> </p> 

## Documentation for

| Category | Value |
|-----|-------------------------------------------------------|
| Vendor Name | DosBox+California Dreams |
| Application Name| Blockout |
| Application Version | ?? (released a really long time ago)|
| Vendor/App Website| https://dosbox.com |


## Vendor Installer Types

This is where we can define the forms of installers available from the vendor. 
<table >
<tr>
<td>

| Type | Available |
|----|----|
| Setup Exe | [<img src="/media/Yes.png" alt="Yes" />](/media/Yes.png) |
| MSI | [<img src="/media/No.png" alt="No" />](/media/No.png) |
| AppX/Bundle | [<img src="/media/No.png" alt="No" />](/media/No.png) |
| MSIX/Bundle | [<img src="/media/No.png" alt="No" />](/media/No.png) |
| .appinstaller | [<img src="/media/No.png" alt="No" />](/media/No.png) |

</td>
<td width=100></td>
<td>

| Architecture | Available |
|----|----|
| 16-bit | [<img src="/media/Yes.png" alt="Yes" />](/media/Yes.png), when supported by DosBox |
| 32-bit | [<img src="/media/Yes.png" alt="Yes" />](/media/Yes.png) |
| 64-bit | [<img src="/media/No.png" alt="No" />](/media/No.png) |
| AnyCPU | [<img src="/media/No.png" alt="No" />](/media/No.png) |
| Arm | [<img src="/media/No.png" alt="No" />](/media/No.png) |
| Arm-64 | [<img src="/media/No.png" alt="No" />](/media/No.png) |

</td>
</tr>
</table>

## App Configuration Type

This is where to place a summary of how application configuration is stored.  Items of configuration of common interest should be documented in a separate file.

| Type | Used |
|----|----|
| Registry | [<img src="/media/No.png" alt="No" />](/media/No.png) |
| File | [<img src="/media/Yes.png" alt="Yes" />](/media/Yes.png) |
| AD/GPO | [<img src="/media/No.png" alt="No" />](/media/No.png) |
| AAD/GPO | [<img src="/media/No.png" alt="No" />](/media/No.png) |


## Repackaging Summary

This is where to list a summary of known success (or not) in repackaging info certain formats.  If repackaging the application is not straightforward, a specific documentation file covering the details for that repackaging format is suggested. Values in the Success field are somewhat subjective, but we recommend that the summary use the following value:

* [<img src="/media/CatFullFidelity.png" alt="Full Fidelity" />](/media/CatFullFidelity.png) - App appears to be completly functional.
* [<img src="/media/CatHighConfidence.png" alt="High Confidence" />](/media/CatHighConfidence.png) - There may be a small loss in functionality, but most companies will be OK with deploying this form.
* [<img src="/media/CatMostlyWorks.png" alt="Mostly Works" />](/media/CatMostlyWorks.png) - A loss in functionality that likely makes this a bad way to deploy.
* [<img src="/media/CatIssues.png" alt="Has Issues" />](/media/CatIssues.png) - Application is known to not work in this form (so far).
* [<img src="/media/CatUnknown.png" alt="Unknown/Untested" />](/media/CatUnknown.png) - No information is available.

| Type | Success |
|----|----|
| MSI | [<img src="/media/CatUnknown.png" alt="Unknown/Untested" />](/media/CatUnknown.png) |
| App-V | [<img src="/media/CatFullFidelity.png" alt="Full Fidelity" />](/media/CatFullFidelity.png) |
| ThinApp | Unkno[<img src="/media/CatUnknown.png" alt="Unknown/Untested" />](/media/CatUnknown.png)wn |
| Citrix App Layers | [<img src="/media/CatUnknown.png" alt="Unknown/Untested" />](/media/CatUnknown.png) |
| Cloud Volumes | [<img src="/media/CatUnknown.png" alt="Unknown/Untested" />](/media/CatUnknown.png) |
| FlexApp | [<img src="/media/CatUnknown.png" alt="Unknown/Untested" />](/media/CatUnknown.png) |
| Numecent | [<img src="/media/CatUnknown.png" alt="Unknown/Untested" />](/media/CatUnknown.png) |
| MSIX | [<img src="/media/CatFullFidelity.png" alt="Full Fidelity" />](/media/CatIssues.png) |

## Useful links
This is a place to put useful links to appropriate existing external sources, either those of the vendor or elsewhere.
