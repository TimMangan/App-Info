# Installation and Configuration Notes for Math Mechanixs

The application is delivered in a setup exe installer or zip.    

## Project Evergreen
Project Evergreen AppTracker does not provide information and sources for installers for this app when last checked.


## ZIP based installer
The ZIP based installer contains a different setup exe than what may be directly downloaded. You use this installer in a two step process, first to download and then to install.  The commands are:
* miktexsetup_standalone.exe --quiet --local-package-repository=C:\miktexRepository --package-set=complete  download
* miktexsetup_standalone.exe --quiet --local-package-repository=C:\miktexRepository  --shared=no --use-registry=yes install

## EXE based installer

It is unknown if the installer supports a silent installation. Documentation on the vendor website pushes the zip based installer for unattended installation.


## SilentInstallHQ
Silent Install HQ provides no information on the silent install of this app.

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* No configuration changes were made in this test.

## Installed Components worth noting

* Installs into UserProgramFiles.
* Also adds files into AppData\Local
* Almost 3000 fonts added.
* Environment Variable PATH updated.
