# Submitting Changes

With github, you should create a free GitHub account first and be logged in. Then you download a copy of the repository to your local machine.  On your machine, you can do what you want just using notepad, but you can also use tools that know about GitHub and the markup syntax.  Microsoft's free VS Code is excellent for this (and you don't need to know a thing about coding).

You can add a new app by adding new folders/files as described below, or you can update information on an existing app file.

When you are ready, you'll submit the changes by using what is called a Pull Request.  This doesn't directly change the site (so don't be afraid), but it sends the changes to us for review and approval.  This is a pretty simple gate-keeper process to keep the site clean.  You'll see an email when the changes are incorporated.

## Templates for adding a new application.

When you add a new app into this repository, you will need to do the following:
* Create a folder for the app (possibly under a folder for the vendor if they have multiple apps).
* Create a ReadMe.md file for the app from this template file.
* Create an InstallConfigure.md file from that template.
* Create a Testing.md file from that template.
* Create one or more Packaging-XXX.md files documenting how you packaged that app and the test results.  Test Results are also summarized in the ReadMe.md file for the app.
* Upload a logo file into the media/AppIcons folder.  This should be a 44x44bit png file.

The purpose of the App ReadMe file is to be the initial page viewed when someone looks for information on this application. It defines:
* The vendor, app, and version, along with a link to the vendor website.
* The types of installers available from the vendor.
* Whether the app stores configuration in file or registry, or may be configured externally.
* A summary of the results from any technology-specific repackage testing that was done (each reported result needs a separate Packaging-XXX file).

This folder contains template files that you can use as a base content to copy into your new file.

## About Markup

Documentation on this site is written in markup and are stored in files ending in the .md file extension.  There is much information online that can help, as well as markup editing tools.

