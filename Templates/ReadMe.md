# Contributing Applications to this Site

The entire point of this site is for IT Pros to be able to contribute their experiences with preparing and deploying applications with their peers.  Together we can make the process much easier through sharing.

GitHub was chosen because, even though we think of it as being for developers, it has features that make it a good fit for documentation.  Microsoft uses GitHub to open source their own documentation, and yes, you can submit fixes to the Microsoft documentation yourself!  But it is free for you to use, you can browse without even having an account or get a free account from GitHub to contribute.  The documentation is build on a simple markup language (actually called `markdown`) that is easy for you to pick up (even in Notepad) and it comes with an infrastructure that makes it easy for you to submit changes into the site.

## Step 1: Get a GitHub account

Start by signing up for a free account.

## Step 2: Look around
The site has a bunch of folders and makrdown files (those are the ones ending in a file extension `.md`).  When you are viewing a folder level, you'll see a list of the files and subfolders under it, and if there is a file in the folder called `readme.md`, the contents of that file are also shown.  This makes the readme file a great place to either provide instruction (as in the case of this one), or an overview of the folder iteself.

Of particular interest
* Ignore the folder called `CodeDontLookHere`!  Yeah, you took a developer course once but you chose to be an IT Professional for a reason.
* Under the `docs` folder is a subfolder `docs/Windows`.  This folder is where all of the documentation for windows apps go.  We might only be interested in Windows apps today, but we're building in for any potential futures too.  Under the Windows folder will be subfolders for each Application.  If there is a vendor that has multiple applications then we'll give them a folder under the Windows folder and put the apps under that.
* Each App folder has a minimum of 4 files (the purpose of which are described below):
* * A `ReadMe.md` file.
* * A `InstallConfiguration.md` file
* * A `Testing.md` file
* * One or more `Packaging-XXX.md` files.
* The Template folder, which contains a template for each of those files so you can easily create your own app.
* When looking at a folder you can see the formatted Readme file, but click on any file to see that file.  Just use the back button on the browser to return to the folder level.
* You can also click on any folder visible, including the App-Info folder to go back to the top level of this repository.
* At the top-level App-Info, the `ReadMe.md` file contains links to each of the applications that we have documented.  As this list grows, you'll want to use the built in search feature - just click the letter `t` on your keyboard to enter search.

| File | Purpose |
|----|----|
| `ReadMe.md` | This file is intended to be a high level description of the application including what kind of app and installers are available from the vendor. We also try to summarize how the app is configured (file/registry/GPO) without details at this level, and summarize the known results from different repackackaging techniques. |
| `InstallConfiguration.md` | This file contains more detailed information on how the app is often installed and configured.  This includes silent installation, and common configuration changes like supressing EULA prompts and defeating updaters built into the app, and package cleanup like removing unnecessary shortcuts. |
| `Testing.md` | This file is critical for each app!!! It defines a simple smoke test that should be used when documenting a `Packaging` result.  The smoke test is not the same as a full-blown User Acceptance Test (UAT), but just the quick and easy test that the packager can use to decide if the package is good enough to move on to UAT. |
| `Packaging-XXX` | Each of these files provides information on a packaging experience using a particular packaging tool or technology.  Information about special things that should be done on this app, and the results of the smoke testing of the application is also included.  We will want you to identify yourself in this file as the contributor.  You can even add an image file of yourself in the `media/contributors` folder and include it in this file as you can see it was done in the template. |

We simplify the interprettion of testing results into four possible result categories:

* The ![badge](https://img.shields.io/badge/-Full%20Fidelity-brightgreen?style=for-the-badge) testing result means that the app contains all of the original application features (except things we want turned off).  Some apps, deployed using certain tools/technologies might loose some minor features, or we may be unable to disable the updater and these do not deserve this result.
* ![badge](https://img.shields.io/badge/-High%20Confidence-green?style=for-the-badge) means that you have high confidence that most companies would still be willing to deploy this app and you should describe the minor issue(s).
* ![badge](https://img.shields.io/badge/-Mostly%20Works-yellow?style=for-the-badge) means that while base functionality works, most companies will probably not deploy this app due to the issues, but there are some that will (because they don't use the feature or have no other choice).  Again, describe the issue(s).
* ![badge](https://img.shields.io/badge/-Major%20Issues-critical?style=for-the-badge) means that there is insufficient functinality for anyone to deploy in this state.
* ![badge](https://img.shields.io/badge/-Unknown%2FUntested-lightgray?style=for-the-badge) result is used when testing results for this scenario are not known.  This is typically used on the application summary readme where we want a consistent looking result summary list.

## Setp 3: Make a simple change

When logged into Github, you can make simple changes directly from your browser.  Let's say you see that Tim made a typo in a document he posted (it's been known to happen).

* Click on the file to view the formatted file.  
* Then click the editor icon at the top of the file (it looks like a pencil) and you'll fall into edit mode.  
* In edit mode, you'll quickly see how headings are done (`#`) as well as bullet lists (`*`). You might also see tables and images in some markdown files.  We even drop into html when we can't seem to get markdown to do exactly what we want.  It's all good!
* Make your changes.
* Preview the results (tab at the top of the editor window). 
* Commit your changes (below the editor window).  Include a short comment, 2 or 3 words, on the change.  There is also a place for a fuller description that might be useful to the reviewer.
* Sumbmit a Pull Request on your commit. This will send your changes for review and request that we pull them into the main branch source of the repository.  This is handled by a volunteer (be patient!) and you'll get an email from GitHub when processed, or if there are questions.

## Step 4: Add a new Application to the repository

You can add new applications in in two ways.

### Adding just from the Browser

You can locally create a folder with the name of your app.  You can create the 4 (or more) files, using the files in this folder starting with names `Template_` as a guide for what to fill in.

You'll want an image for the app to make it look nice.  This is usually taken from the shortcut, but wherever you can get one we'd like a png or jpg file that is 44x44 pixels in size.  Commit the change and make a Pull Request.

When ready, go to the website and browse to the folder `media\AppIcons`. Click on the `Add File` pull-down and select upload file.  Select your image.

Then browse to the `docs/Windows` folder.  Click on the `Add File` pull-down and select upload file. This time select your application folder.  Commit and make the Pull Request.

### Adding using tooling

The other option is to use GitHub as the source control system it is.  You download the entire repository to a folder on your local system. You can then use a free tool like Microsoft `VS Code` to provide a markdown editor and manage the process of keeping your local copy in sync with changes by others and make it easy to submit and manage your commits and pull requests.

In VS Code, you'd right click on a that Windows folder to add your app folder. Drag-and Drop the template files (holding down the shift key to copy) from the template folder to your app folder.  Right click on the copied files to rename them. And then click on a file to edit it. You'll want to add a markdown extension to VS Code (I'm using `Markdown Preview Github Styling`) to make the editing easier.  Drag and drop your graphic file from an explorer window and drop it on that AppIcons folder.

When everything is saved, click on the branch icon on the left of VSCode and click the + next to each file to stage the changes.  When all changes are staged, make the commit and then synchronize to create the pull request.




