# Testing CyberDuck

The following tests should be considered to determine the application fidelity when repackaging.

* Installation involves a service.  Verify if Bonjour service is present and running by using the Windows Services Control Panel (services.msc)
* One shortcuts should be present.
* Launch app from shortcut.
* Connect to an appropriate resource and test appropriately.  For example, for an FTP Site:
* * Make a connection.
* * Drag and drop a file from an external windows explorer window onto a folder on the ftp site. Make sure it copies.
* * Edit a text based file on the FTP site by rightclick and open in notepad.  Make a change in notepad and save the file.  It should automatically update the FTP site.
