# App-Info Document ACDC (v2)

[<img src="/media/AppIcons/LOGINACDCTwo-Square44x44Logo.scale-100.png" align="left" alt="ACDC logo"  />](/media/AppIcons/LOGINACDCTwo-Square44x44Logo.scale-100.png) ACDC Version 2 is a help-desk tool for use on end-user systems that are using Microsoft App-V Versions 5 through 5.2.  It supports local configuration of the App-V Client and troubleshooting and repair functionality for applications virtualized under App-V.  (ACDC V1 supported App-V 4.x systems).


This is the high level file that describes the application summary.  Additional documentation files may also be present to cover specific scenarios, such as repackaging into a specific format. 

## Documentation for

| Category | Value |
|-----|-------------------------------------------------------|
| Vendor Name | Login Consultants |
| Application Name| ACDC V2 |
| Application Version | 3.0.0.3 (released 2015/03, latest version available)|
| Vendor/App Website| https://www.loginconsultants.com |



## Vendor Installer Types

This is where we can define the forms of Windows installers available from the vendor. 
<table >
<tr>
<td>

`Note`: Linux and Mac releases are also available.

| Type | Available |
|----|----|
| Zip | [<img src="/media/Yes.png" alt="Yes" />](/media/Yes.png) |
| Setup Exe | [<img src="/media/No.png" alt="No" />](/media/No.png |
| MSI | [<img src="/media/No.png" alt="No" />](/media/No.png |
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
| AnyCPU | [<img src="/media/No.png" alt="No" />](/media/No.png) |
| Arm | [<img src="/media/No.png" alt="No" />](/media/No.png) |
| Arm-64 | [<img src="/media/No.png" alt="No" />](/media/No.png) |

</td>
</tr>
</table>

## App Configuration Type

This is where to place a summary of how application configuration is stored.  The application has no configuration of it's own.

| Type | Used |
|----|----|
| Registry | [<img src="/media/No.png" alt="No" />](/media/No.png) |
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
| MSIX |  [<img src="/media/CatFullFidelity.png" alt="Full Fidelity" />](/media/CatFullFidelity.png) |

## Useful links
This is a place to put useful links to appropriate existing external sources, either those of the vendor or elsewhere.
