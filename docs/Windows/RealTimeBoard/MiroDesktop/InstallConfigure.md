# Installation and Configuration Notes for Miro

 The vendor really wants to install the app into LocalAppData

## Project Evergreen
Project Evergreen AppTracker does not provide information and sources for installers for this app when last checked.

## SilentInstallHQ

Silent Install HQ provides no information on the silent install of this app.

## EXE Install
The exe installer appears to have no command line arguments.  It installs itself passively.  This install will go into the user's AppData\Local\RealTimeBoard folder.

## MSI Install
This installer will install itself into the Program Files (x86) folder, but what it installs appears to be a per-user installer that is different than the EXE installer also provided by the vendor.  It adds an entry into the Windows registry "Run" key as a way to run that installer upon user logon with this command:

    "C:\Program Files\Miro Installer\RealtimeBoard.exe" --checkInstall

The vendor website indicates that this command checks to see if the Mira Desktop app is installed (we think by looking for the files), and then installs Mira Desktop into the user's AppDataLocal folder. If the MSI version is selected with updates we suspect that the Miro Installer also performs that check.

Also note that the Miro Installer program will return immeditely and perform the installation of Mira Desktop in the background, so any installation scripting may want to sleep a few minutes to let that complete.

## Manual Install
* Create a folder, such as `C:\Program Files\ReverseDNS`.
* Copy the exe file into that folder.
* Create a shortcut to the executable.

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* None, except or default language if needed.

## Installed Components worth noting
 
* The application installs into program files.
* There is one shortcut.
* There  are no FTA, shell extensions, protocol handlers, or services.
