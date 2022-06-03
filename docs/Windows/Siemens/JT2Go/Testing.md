# Testing JT2Go

The following tests should be considered to determine the application fidelity when repackaging.

* Launch app, there should be no upgrade prompt or eula.
* Change a config(File-->Preferences-->3D Loader-->Other-->Show Load Failure Dialogs), confirm it is sticky.
* Open file in TestResources-DWG. Make sure you can open the file. There is no FTA so this is done from the file menu of the app.
* Reopen app. In the funky center menu, pick the showcase and select an app.  The browser should offer to Open it.  Say yes (You will have to verify that it is OK).  This tests the protocol handler.