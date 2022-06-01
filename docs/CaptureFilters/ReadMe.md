# Capture Filters

In addition to application specific information, we'd like to gather the collective wisdom of the community on setting up capture filters and package cleanup.

During application installation capture, the application installer may add file and registry items that are not necessary in the resultant package.  Additionally, other running software on the capture device may cause file or registry activity that is captured by mistake.  

Preventing unintended capture, or cleaning up the package, is very important when the resulting package is an MSI as those components will be installed and integrated onto systems receiving this package and may break other applications or the OS itself.  In situations for packaging for runtimes that will be containerized, such as for Microsoft App-V, MSIX, or other layering products, there is less danger in including these unintended captures.  However, it is considered to be a best practice to keep the package as clean as practical.

Most capturing tools have some sort of filter that may be applied to help with this.

This folder is the highest level folder for information on setting up application capture filters. Please use appropriate subfolders to add your own submissions.  It is important not only to document the items we typically want cleaned out of repackaging efforts, but to:

* Document what the thing(s) is/are being removed.
* Why it isn't needed.
* Any special situations where it should not be removed.



