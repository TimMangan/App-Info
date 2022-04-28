# App-Info Document DosBox_Blockout

This is the high level file that describes the application summary.  Additional documentation files may also be present to cover specific scenarios, such as repackaging into a specific format. 

## Documentation for

| Category | Value |
|-----|-------------------------------------------------------|
| Vendor Name | DosBox+Apogee |
| Application Name| Blockout |
| Application Version | ?? (released a really long time ago)|
| Vendor/App Website| https://dosbox.com |

## Application Purpose

This application is an example of a 16-bit DOS application, which natively could no longer run on x64 systems.  We use DosBox as a way to host this app; packaging them together.

Blockout is just a Tetris like game, but the concept here holds for a bunch of old 16-bit business apps that are still in use today, mostly by Small companies.

## Vendor Installer Types

This is where we can define the forms of installers available from the vendor. 

| Type | Available |
|----|----|
| Setup Exe | Yes |
| MSI | No |
| AppX/Bundle | No |
| MSIX/Bundle | No |
| .appinstaller | No |

| Architecture | Available |
|----|----|
| 16-bit | Yes, when supported by DosBox |
| 32-bit | Yes |
| 64-bit | No |
| AnyCPU | No |
| Arm | No |
| Arm-64 | No |

## App Configuration Type

This is where to place a summary of how application configuration is stored.  Items of configuration of common interest should be documented in a separate file.

| Type | Used |
|----|----|
| Registry | No |
| File | Yes |
| AD/GPO | No |
| AAD/GPO | No |


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
