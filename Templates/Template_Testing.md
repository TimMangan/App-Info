# Testing APP

The purpose of the Testing file is to document a "smoke test" verification of the packaged app.  Such a test is generally focused on ensuring that the installed repackaged app is completely present, including the various forms of application access (like Shortcuts, FTAs, Shell Extensions, and Protocol Handlers), that the app starts up reasonably (such as without EULA or Updaters), and that personal settings of the app may be made and saved.  Each app should have a Testing file.

This style of test is usually different than a User Acceptance Test, which focuses on ensuring full functionality to perform the task. 

Please remove the boiler plate at and above this line, then edit the example below.

The following tests should be considered to determine the application fidelity when repackaging.

* XXX shortcuts should be present.
* Launch the app.
* * There should be no EULA displayed.
* * User should not be prompted for updates.
* * Verify app is configured as desired (if any).
* * Verify ability to change app configuration, close and ensure changes stick.
* Check FTAs by viewing a .XXX file.
* Other...
