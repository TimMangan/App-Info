# Installation and Configuration Notes for R and RStudio

By default the app will install under a `R` folder in the Program Files folder.

Install the R language first, then RStudio using the zip installation..

## Project Evergreen
Project Evergreen AppTracker provides information and sources for installers for RStudio only https://stealthpuppy.com/apptracker/#rstudio

## EXE based R language installer

The EXE installer for R (Language) may be silently installed:
 * For example: '/SP- /SILENT /SURPRESSMSGBOXES '
The application has file-based configuration that is not generally used.

## EXE based installation of RStudio.
Use '/S' for a silent installation.

##  ZIP based installation of RStudio.
Unpack into "$($env:ProgramFiles)\R"

## SilentInstallHQ

Silent Install HQ provides no information on the silent install of this app.

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* Preconfiguration is possible by grabing two files in AppData\Roaming\RStudio for use in your installation script.
* * `crash-handler.conf` Can disable sending crash logs to the internet.  Launch app to create the initial file.
* * `rstudio-prefs.json` Can disable updates and/or set other settings.  Use the Tools menu Global Settings to create the initial file.

## Installed Components worth noting
 
* The application installs into program files.
* There are two shortcuts installed, one for 32-bit and one for 64-bit. They both point to an exe named RGui.exe in different folders.
* There is a new FTA (.RData) that has a shell integration verb command.
* There are no shell extensions, protocol handlers, or services.
