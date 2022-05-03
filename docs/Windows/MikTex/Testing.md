# Testing Math Mechanixs

The following tests should be considered to determine the application fidelity when repackaging.

* Verify number of shortcuts present (6, unless some were removed).
* Lauch primary app MikTex (TexWorks).
* * Change icon settings in the menu Edit->Preferences. Close/reopen and verify that changes appear.
* * Use menu Help-->Settings and resources, click on link to ensure that AppData\Local was mapped.
* Open a sample .tex file using the FTA command verb.
* * Click the Typeset button in the open document. NOTE: There will be a prompt to "install" a component, but this is not a product install as much as an install from the product to a file in the folder containing what is needed. After this, Pdf should render into a new window.

