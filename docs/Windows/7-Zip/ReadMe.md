# App-Info Document 7-Zip

<div>

<img src="/media/AppIcons/SevenZFM-256.png" align="left" valign="top"  height="256" alt="7-Zip logo"  /> 7-zip is a freeware version of an archive (aka "Zip") compression/decompression tool issued via GNU license. It also has open-source code available.  

<p> </p>

This software is popular among IT Pros because it also includes the ability to extract files from inside of WinPE files.  For example, such as to access embedded MSI from the setup.exe installers.  Ot so extract icons and other resources from an exe or dll file.

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

| Type | Available |
|----|----|
| Setup Exe | [<img src="/media/Yes.png" alt="Yes" />](/media/Yes.png) |
| MSI | [<img src="/media/Yes.png" alt="Yes" />](/media/Yes.png) |
| AppX/Bundle | [<img src="/media/No.png" alt="No" />](/media/No.png) |
| MSIX/Bundle | [<img src="/media/No.png" alt="No" />](/media/No.png) |
| .appinstaller | [<img src="/media/No.png" alt="No" />](/media/No.png) |

</td>
<td width=100></td>
<td>

| Architecture | Available |
|----|----|
| 32-bit | [<img src="/media/Yes.png" alt="Yes" />](/media/Yes.png) |
| 64-bit | [<img src="/media/Yes.png" alt="Yes" />](/media/Yes.png) |
| AnyCPU | [<img src="/media/Unknown.png" alt="Unknown" />](/media/Unknown.png) |
| Arm | [<img src="/media/No.png" alt="No" />](/media/No.png) |
| Arm-64 | [<img src="/media/Yes.png" alt="Yes" />](/media/Yes.png) |

</td>
</tr>
</table>

## App Configuration Type

This is where to place a summary of how application configuration is stored.  Items of configuration of common interest should be documented in a separate file.

| Type | Used |
|----|----|
| Registry | [<img src="/media/Yes.png" alt="Yes" />](/media/Yes.png) |
| File | [<img src="/media/No.png" alt="No" />](/media/No.png) |
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
| ThinApp | [<img src="/media/CatUnknown.png" alt="Unknown/Untested" />](/media/CatUnknown.png) |
| Citrix App Layers | [<img src="/media/CatUnknown.png" alt="Unknown/Untested" />](/media/CatUnknown.png) |
| Cloud Volumes | [<img src="/media/CatUnknown.png" alt="Unknown/Untested" />](/media/CatUnknown.png) |
| FlexApp | [<img src="/media/CatUnknown.png" alt="Unknown/Untested" />](/media/CatUnknown.png) |
| Numecent | [<img src="/media/CatUnknown.png" alt="Unknown/Untested" />](/media/CatUnknown.png) |
| MSIX | [<img src="/media/CatHighConfidence.png" alt="High Confidence" />](/media/CatHighConfidence.png) on 10, [<img src="/media/CatFullFidelity.png" alt="Full Fidelity" />](/media/CatFullFidelity.png) on 11 |

## Useful links
This is a place to put useful links to appropriate existing external sources, either those of the vendor or elsewhere.
