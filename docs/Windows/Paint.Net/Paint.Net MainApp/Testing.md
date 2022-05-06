# Testing Notepad++

The following tests should be considered to determine the application fidelity when repackaging.

* One shortcut should be present.
* Launch app from shortcut.  
* * There should be no update detected (shows in the title bar of the app).
* * Make a configuration change (e.g.: View-->Inches).Close/Reopen/Verify Sticky.
* Check FTAs using a variety of file types by looking at the files in Explorer medium/large icon size.  ICO and TGA should have an icon with a paintbrush. .psd is a generic white icon.  Several others should have a thumbnail of the image.  Double-Click on .tga and .pdn should open Paint.Net.
