# Installation and Configuration Notes
By default the app will install into a `7-Zip` folder under the apprpriate Program Files folder.

## Exe based installer

Silent installation is possible:  

* "/S" (capitalized) for silent installation. 

## MSI based installer

Normal MSI parameters are available for quick/passive/silent installation, and:

* INSTALLDIR is supported.
* ALLUSERS is supported.

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* The product does not currently have an autoupdater built in.
* Registry based configuration available under the key `[HKEY_CURRENT_USER\SOFTWARE\7-Zip\FM]`.  None of these items appear critical.

## Installed Components worth noting

* The application installs with two shortcuts, one for the program and another for the chm-based help file.  The help is alao available from in the program so the latter shortcut may be removed.
* The application adds/updates a lot of file type associations for compressed file formats.  Most of these are for Shell Integration (verb/command) access.
* The application has several shell extensions:
* * 2 Context Menu handlers (one for all file types and another for Directories).
* * A Drag&Drop handler.
* The application includes an App Paths registration for both search (execution alias) and dll loading.