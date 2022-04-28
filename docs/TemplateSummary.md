# App-Info Document Template (replace this with your application name)

This is the high level file that describes the application summary.  Additional documentation files may also be present to cover specific scenarios, such as repackaging into a specific format.  Make a copy of this template saved into an appropriate subfolder and name it **ReadMe.md**.

## Documentation for

| Category | Value |
|-----|-------------------------------------------------------|
| Vendor Name | |
| Application Name| |
| Application Version | Leave blank if version specific doc files exist. |
| Vendor/App Website|  |

| Architecture | Available |
|----|----|
| 32-bit | Unknown |
| 64-bit | Unknown |
| AnyCPU | Unknown |
| Arm | Unknown |
|Arm-64 | Unknown |

## Application Purpose

This application is used for ...

## Vendor Installer Types

This is where we can define the forms of installers available from the vendor.

| Type | Available |
|----|----|
| Setup Exe | Unknown |
| MSI | Unknown |
| AppX/Bundle | Unknown |
| MSIX/Bundle | Unknown |
| .appinstaller | Unknown |

## App Configuration Type

This is where to place a summary of how application configuration is stored.  Items of configuration of common interest should be documented in a separate file.

| Type | Used |
|----|----|
| Registry | Unknown |
| File | Unknown |
| AD/GPO | Unknown |
| AAD/GPO | Unknown |


## Repackaging Summary

This is where to list a summary of known success (or not) in repackaging info certain formats.  If repackaging the application is not straightforward, a specific documentation file covering the details for that repackaging format is suggested. Values in the Success field are somewhat subjective, but we recommend that the summary use the following value:

* `Full Fidelity` - App appears to be completly functional.
* `High Confidence` - There may be a small loss in functionality, but most companies will be OK with deploying this form.
* `Mostly Works` - A loss in functionality that likely makes this a bad way to deploy.
* `Issues` - Application is known to not work in this form (so far).
* `Unknown` - No infomration is available.


| Type | Success |
|----|----|
| MSI | Unknown |
| App-V | Unknown |
| ThinApp | Unknown |
| Citrix App Layers | Unknown |
| Cloud Volumes | Unknown |
| FlexApp | Unknown |
| Numecent | Unknown |
| MSIX | High Confidence |

## Useful links
This is a place to put useful links to appropriate existing external sources, either those of the vendor or elsewhere.
