# Testing 7-Zip

The following tests should be considered to determine the application fidelity when repackaging.

* Two shortcuts should be present (unless the chm is not desired).
* Launch the app.
* Verify app is configured as desired (if any).
* Verify ability to change app configuration, close and ensure changes stick.
* Check FTAs by viewing a .7z file.
* Verify icons of .Zip files in explorer show as desired.
* Look for a context menu when right-click on a DIRECTORY (look for 7-zip in the menu list).
* Look for a Context menu when right-click on a file (look for things like create name.zip or update name.zip or add to name.zip).
* Drag and drop a file onto a .7z file and ensure file is added.
* If help shortcut is published, test it.