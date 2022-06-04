# Installation and Configuration Notes for Snagit

By default the app will install into the program files folder by default.


## MSI installer 

The primary installer supports passive and silent installation.  This may be performed using the transform file. Techsmith provides a tool to help you create the transform file and it supports full configuration of the installation.
* The Techsmith Deployment Tool may be used to configure the application by creating an MST file for the installer.  See https://assets.techsmith.com/Downloads/accessories/TechSmith_Deployment_Tool_Documentation.pdf 
* * You may want to disable the "Run Snagit when Windows starts" feature.  This feature might not work in some environments like MSIX.
* * You likely will want to check several items on the "Disable Snagit Settings" page:
* * * "Disable automatic updates", 
* * * "Disable TechSmith notification feed", 
* * * "Disable usage reporting", 
* * * "Disable TechSmith account sign-in",
* * * "Disable Output Manager".
* * For capture to containerized environments, uncheck the Snagit Printer box as this feature installs a printer driver.
* * You may want to disable some of the outputs also, such as Techsmith Relay.  Outputs are interfaces that output the capture into another program.
* * You likely want to disable the "Techsmith Fuse" feature, especially for App-V.  This allows the user to install a phone app and send output to this app via a service.
* * You likely want to accept the EULA on behalf of users.

* For the msi installation, use arguments 'TRANSFORMS="snagit.mst" DISABLEADVTSHORTCUTS=1 /passive /promptrestart' for a passive installation.  Substitute '/q' for '/passive' for a silent installation.

It is important to disable the autoupdater (for other than MSI packaging). Certain features do not work under App-V or MSIX, however these are features that the enterprise often prefers to disable anyway.

## SilentInstallHQ

Silent Install HQ provides no information on the silent install of this app. 

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* See information above on using the Deployment Tool to create a transform file.

## Installed Components worth noting

* The program installs mostly into Program Files.
* The program installs items into C:\ProgramData, as well as the user LocalAppData and AppData (Roaming).
* The program installs licening in the C:\Users\TechSmith area.
* There are two shortcuts, one for the Snagit Capture program and the other for the Editor.
* There are many standard and 2 special FTAs.
* There is a shell extension for ContextMenu shared for the special "*" and "Directory" FTA.
* There is a shell extension for Thumbnail Handler for the .snag file type.
* There are three protocol handlers.
* There are no services.
* There is an App Paths registration for dll load order for Snagit.
* This is an App Paths registration for exe search (applicaiton alias) for SnagIt.
* There is a RegisteredApplications registration.
* There is a run key to launch snagit (unless disabled).
* There are fonts.