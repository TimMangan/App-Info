# Testing ConEmuPack

The following tests should be considered to determine the application fidelity when repackaging.

* Installs with 1 shortcut.
* Launch. Make sure the top right of the window does not show that a newer version is available.
* Check any other configuration you may have set.
* Modify the configuration (Hamburger menu).  When the dialog appears, if it cannot get write access to the xml configuration file, the save button will be disabled.  Ensure the user can make configuration changes.  Close the app and start again and check if the configuration changes stuck.