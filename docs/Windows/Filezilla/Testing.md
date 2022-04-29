# Testing Filezilla

The following tests should be considered to determine the application fidelity when repackaging.

* One shortcut should be present (assuming uninstall was removed).
* Launch Filezilla app from shortcut.  
* Ensure no updates are detected.
* In Site Manager, add a new site.  Configure to attach to a test FTP site; connect and make sure data is present.
* Close and reopen tool and ensure site is still present in the Site Manager.
* Attach again to test site. Drag and drop a folder from an explorer window into the site.  Copy it back out to another local location in explorer.
* right click on a file on the ftp file that is a text file (txt, xml, log, etc...).  Ensure it transfers over and modify the file.  When you save the file locally, Filezilla should detect this and offer to transfer it back. 
