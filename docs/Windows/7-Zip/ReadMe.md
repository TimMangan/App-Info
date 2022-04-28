# App-Info Document 7-Zip

This is the high level file that describes the application summary.  Additional documentation files may also be present to cover specific scenarios, such as repackaging into a specific format. 

## Documentation for

| Category | Value |
|-----|-------------------------------------------------------|
| Vendor Name | 7-Zip (Igor Pavlov) |
| Application Name| 7-Zip |
| Application Version | 19.00 (released 2019/02, newer versions available)|
| Vendor/App Website| www.7-zip.org |

## Application Purpose

This application is a freeware version of an archive (aka "Zip") compression/decompression tool issued via GNU license.  It has open-source code available.  It is popular among IT Pros as it also includes the ability to extract files from inside of WinPE files, such as to access an embedded MSI from the setup.exe installer, or icons from an exe or dll.

## Vendor Installer Types

This is where we can define the forms of installers available from the vendor.

| Type | Available |
|----|----|
| Setup Exe | Yes |
| MSI | Yes |
| AppX/Bundle | No |
| MSIX/Bundle | No |
| .appinstaller | No |

| Architecture | Available |
|----|----|
| 32-bit | Yes |
| 64-bit | Yes |
| AnyCPU | ? |
| Arm | No |
| Arm-64 | Yes |

## App Configuration Type

This is where to place a summary of how application configuration is stored.  Items of configuration of common interest should be documented in a separate file.

| Type | Used |
|----|----|
| Registry | Yes |
| File | No |
| AD/GPO | No |
| AAD/GPO | No |


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
| App-V | Full Fidelity |
| ThinApp | Unknown |
| Citrix App Layers | Unknown |
| Cloud Volumes | Unknown |
| FlexApp | Unknown |
| Numecent | Unknown |
| MSIX | High Confidence |

## Useful links
This is a place to put useful links to appropriate existing external sources, either those of the vendor or elsewhere.
