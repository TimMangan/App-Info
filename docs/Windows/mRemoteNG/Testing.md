# Testing mRemoteNG

The following tests should be considered to determine the application fidelity when repackaging.

* Make sure the native LocalAppData `mRemoteNG` folder is cleared out prior to testing.
* One (or more if not removed) shortcut should be present.
* Launch app from shortcut.  
* * Withoug preconfig, updates will appear.  Turn off in preconfig, but an oobe configuration prompt will appear anyway. This cannot be helped.
* * Verify settings per any preconfiguration. 
* * Change a setting, close, reopen and verify settings change stick.
* * Make a remote connection. 
* * Close and reopen app, make sure connection remains in the list.
