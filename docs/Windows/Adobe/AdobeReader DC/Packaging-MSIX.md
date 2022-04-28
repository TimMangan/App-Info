# Packaging AdobeReader DC for MSIX

The app has been packaged in MSIX with the PSF.

* PsfLauncher is required as is the FRF.

Testing on Windows 10/11 indicates `Mostly Works`, and any company considering MSIX deployment should througly test the package.  

* Internet Explorer integration is not possible with MSIX.  When this is not an issue at your company, the validation is raised to `High Confidence`.
* The other most noticable issue is that the License Agreement popup appears.
