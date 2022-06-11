# Testing WinSCP

The following tests should be considered to determine the application fidelity when repackaging.

* There should be one shortcut (assuming desktop was removed).
* Launch app and check preconfig
* Connect to an ftpsite (or even just get an access denied from a real one)
* Save a site in the configuration, close/reopen app and ensure sticky.
* Test protocol handler (type dav:\\servername from a web browser.  Should switch apps to winscp.  It's OK if the site doesn't exist as long as you get an error from WinSCP.
* Test a .filetype (from TestResrouces folder).
* Test Copyhook handler by copying a file from a site to the local system (network requires configuration).