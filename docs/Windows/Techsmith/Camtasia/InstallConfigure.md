# Installation and Configuration Notes for Camtasia

By default the app will install into the program files folder by default.

## Project Evergreen
Project Evergreen AppTracker provides information and sources for installers for this app https://stealthpuppy.com/apptracker/#techsmithcamtasia 


## EXE Dependency based installer for WebView2

The product requires Microsoft Edge WebView2 as a dependency.  This is provided as an exe installer

The dependency exe installer supports silent installation:
* Use '/silent /install' for silent installation.

To determine if this dependency is already present, test for
    'HKLM:\SOFTWARE\WOW6432Node\Microsoft\EdgeUpdate\Clients\{F3017226-FE2A-4295-8BDF-00C3A9A7E4C5}'

## EXE Dependency based installer for VC redistributables

The product requires VC redistributables (x64 14.29.301330) as a dependency.  This is provided as an exe installer

The dependency exe installer supports silent installation:
* Use '/quiet /install' for silent installation.

## MSI Main installer 

The primary installer supports passive and silent installation.  This may be performed using the transform file. Techsmith provides a tool to help you create the transform file and it supports full configuration of the installation.
* The Techsmith Deployment Tool may be used to configure the application by creating an MST file for the installer.  See https://assets.techsmith.com/Downloads/accessories/TechSmith_Deployment_Tool_Documentation.pdf
* For the msi installation,use arguments 'TRANSFORMS="camtasia.mst" DISABLEADVTSHORTCUTS=1 /passive /promptrestart' for a passive installation.  Substitute '/q' for '/passive' for a silent installation.

It is important to disable the autoupdater (for other than MSI packaging). Certain features do not work under App-V or MSIX, however these are features that the enterprise often prefers to disable anyway.

## SilentInstallHQ
Silent Install HQ provides no information on the silent install of this app. 

## Typical Configuration Items 

This identifies the most commonly interesting configuration items in the application.

* The product does have an autoupdater, but it may be disabled in the installer.
* 

## Installed Components worth noting

* The program installs mostly into Program Files.
* Edge Webview2 Dependency may install into Program Files (x86).
* Program Data (Common AppData) is used.
* The C:\Users\Public\Techsmith folder is used for licensing.
* There are two shortcuts, one for Studio and the other the Recorder.
* There are 9 FTAs, mostly with a Shell Integration Verb command.
* There is a shell extension for ContextMenu for the .trec FTA.
* There are two protocol handlers.
* There are no services.
* There are fonts.