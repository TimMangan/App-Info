# Testing Fiddler

The following tests should be considered to determine the application fidelity when repackaging.

* Two shortcuts should be present.
* Launch primary Fiddler app from shortcut.  
* You may notice a warning about it beind an old version and do you want to check for updates. Ignore.
* There should be no prompt to join CEP program (if disabled via registry as part of the install).
* There should be no prompt for the imersive container setting (assuming taken care of via registry settings during install).
* The font settins should be at 10pt (assuming taken care of via registry settings during install).
* Verify that you can modify a setting, close/reopen Fiddler and ensure the change sticks.
* Open a browser to confirm that you can scan traffic.
* Click WinConfig.  There should be items in the list not present on the client, so say OK to those, select all and save. This should not fail due to lack of elevation.
