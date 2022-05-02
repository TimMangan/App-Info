# App-Info Document Template (replace this with your application name)

When you add a new app into this repository, you will need to do the following:
* Create a folder for the app (possibly under a folder for the vendor if they have multiple apps).
* Create a ReadMe.md file for the app from this template file.
* Create an InstallConfigure.md file from that template.
* Create a Testing.md file from that template.
* Create one or more Packaging-XXX.md files documenting how you packaged that app and the test results.  Test Results are also summarized in the ReadMe.md file for the app.
* Upload a logo file into the media/AppIcons folder.  This should be a 44x44bit png file.

The purpose of the App ReadMe file is to be the initial page viewed when someone looks for information on this application. It defines:
* The vendor, app, and version, along with a link to the vendor website.
* The types of installers available from the vendor.
* Whether the app stores configuration in file or registry, or may be configured externally.
* A summary of the results from any technology-specific repackage testing that was done (each reported result needs a separate Packaging-XXX file).

Please remove the boiler plate at and above this line, then edit the example below.
_____

[<img src="/media/AppIcons/Template.png" align="left" alt="XXX logo"  />](/media/AppIcons/Template.png)  This application is used for XXX...

This is the high level file that describes the application summary.  Additional documentation files may also be present to cover specific scenarios, such as repackaging into a specific format. 

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

| Type | Available |
|----|----|
| Setup Exe | [<img src="/media/Unknown.png" alt="Unknown" />](/media/Unknown.png) |
| MSI | [<img src="/media/Unknown.png" alt="Unknown" />](/media/Unknown.png) |
| AppX/Bundle | [<img src="/media/Unknown.png" alt="Unknown" />](/media/Unknown.png) |
| MSIX/Bundle | [<img src="/media/Unknown.png" alt="Unknown" />](/media/Unknown.png) |
| .appinstaller | [<img src="/media/Unknown.png" alt="Unknown" />](/media/Unknown.png) |

</td>
<td width=100></td>
<td>

| Architecture | Available |
|----|----|
| 32-bit | [<img src="/media/Unknown.png" alt="Unknown" />](/media/Unknown.png) |
| 64-bit | [<img src="/media/Unknown.png" alt="Unknown" />](/media/Unknown.png) |
| AnyCPU | [<img src="/media/Unknown.png" alt="Unknown" />](/media/Unknown.png) |
| Arm | [<img src="/media/Unknown.png" alt="Unknown" />](/media/Unknown.png) |
| Arm-64 | [<img src="/media/Unknown.png" alt="Unknown" />](/media/Unknown.png) |

</td>
</tr>
</table>

## App Configuration Type

This is where to place a summary of how application configuration is stored.  Items of configuration of common interest should be documented in a separate file.

| Type | Used |
|----|----|
| Registry | [<img src="/media/Unknown.png" alt="Yes" />](/media/Unknown.png) |
| File | [<img src="/media/Unknown.png" alt="Yes" />](/media/Unknown.png) |
| AD/GPO | [<img src="/media/Unknown.png" alt="Yes" />](/media/Unknown.png) |
| AAD/GPO | [<img src="/media/Unknown.png" alt="Yes" />](/media/Unknown.png) |


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
| App-V | [<img src="/media/CatUnknown.png" alt="Unknown/Untested" />](/media/CatUnknown.png) |
| ThinApp | [<img src="/media/CatUnknown.png" alt="Unknown/Untested" />](/media/CatUnknown.png) |
| Citrix App Layers | [<img src="/media/CatUnknown.png" alt="Unknown/Untested" />](/media/CatUnknown.png) |
| Cloud Volumes | [<img src="/media/CatUnknown.png" alt="Unknown/Untested" />](/media/CatUnknown.png) |
| FlexApp | [<img src="/media/CatUnknown.png" alt="Unknown/Untested" />](/media/CatUnknown.png) |
| Numecent | [<img src="/media/CatUnknown.png" alt="Unknown/Untested" />](/media/CatUnknown.png) |
| MSIX | [<img src="/media/CatUnknown.png" alt="Unknown/Untested" />](/media/CatUnknown.png) |

## Useful links
This is a place to put useful links to appropriate existing external sources, either those of the vendor or elsewhere.
