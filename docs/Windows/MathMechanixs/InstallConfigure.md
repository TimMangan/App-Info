# Installation and Configuration Notes for Math Mechanixs

The application is delivered in a setup exe installer.  

## Project Evergreen
Project Evergreen AppTracker does not provide information and sources for installers for this app when last checked.


## EXE based installer

Installer supports a silent installation:
* Use '/silent'


## SilentInstallHQ
Silent Install HQ provides no information on the silent install of this app.

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* No configuration changes were made in this test.
* Several of the shortcuts would likely be removed, such as unintaller and shortcuts to websites.
* In a repackaged scenario, it is possible to add two files into the user's AppData/Roaming folder to pre-configure the app.
* `Roaming/Math Machanixs/Math Mechanixs/MathMechanixs.ini` contains settings to disable autoupdate, as well as other first time activities including a EULA, Tutorial, and Tip of the Day.  You can run the app once and configure it via the GUI to capture this file.
* `Roaming/Math Machanixs/Math Mechanixs/MathMechanixsUser.lib` is actually a text based file. You should copy this into the package if you copy the ini file.  By default, it does nothing, but it appears that you could add/preconfigure some libraries for a classroom setting that requires them.

## Installed Components worth noting

* 6 shortcuts are installed by default.
* 1 FTA (.mtx) with Shell Integration Command
* No Shell Extensions, Protocol Handlers, or Services.
* The app installer does not install anything in the user's AppData\Local or Roaming folders.
