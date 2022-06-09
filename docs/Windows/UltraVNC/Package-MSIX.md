# Packaging UltraVNC for MSIX

The software was packaged on Windows 10 21H2 using Microsoft MSIX Packaging Tool 1.2022.512 and likely requires no special treatment.
* The MMPT will, by default, ignore the duplicate desktop shortcuts.  It will also, by default, ignore the shortcut to the program installation folder.  This is probably desirable.  If the latter is reqired, PsfLauncher will be needed.



Testing on Windows 10/11 indicates ![badge](https://img.shields.io/badge/-Major%20Issues-critical?style=for-the-badge)) support of the app.


# WIP
Starting the 'Settings" it tried to find a native key HKLM\System\CurrentControlSet\Services\bam\UserSettings\S-1-5-21-..-1105 which it finds, and then query value on same\UltraVNC_hash which it does not! There appear to be values in this form for other packages, but not this one.  I also see "white" on the start menu.

## Contributors

| Contributor | Name | Date |
|----|----|----|
| [<img src="/media/Contributors/TimMangan.jpg" align="left" Height="128" />](/media/Contributors/TimMangan.jpg) | TimothyMangan | June 2022 |

