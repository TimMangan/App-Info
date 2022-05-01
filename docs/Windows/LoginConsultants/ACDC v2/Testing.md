# Testing ACDC (V2)

The following tests should be considered to determine the application fidelity when repackaging.

* Launch the app using 'Run as Administrator'.
* * Ensure the App-V Client is enabled, if not enable it.
* * Change a configuration option to the App-V Client.
* * Close/Reopen and ensure setting is still present.
* Launch app normally as standard user.
* * If configured with an App-V Publishing Server, refresh applications.
* * Run a different App-V app and change configuration in it and close it.
* * In ACDC, perform a data repair on that app. Then restart the app and verify previous configuration change is gone.

