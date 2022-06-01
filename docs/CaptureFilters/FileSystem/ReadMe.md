# Capture Filters: FileSystem

This is the folder for information on setting up application capture filters for files and folders.

It is important not only to document the items we typically want cleaned out of repackaging efforts, but to:

* `Entry`: Document what the thing(s) is/are being removed.
* `Explanation`: What is is/Why it isn't needed.
* `Exceptions`: Any special situations where it should not be removed.

The information provided assumes packaging on x64 systems.

## System's AppData Local area  (VFS\Common Appdata)
| Entry | Explanation | Exceptions |
|----|----|----|
| %ProgramData%\Microsoft\AppV | Microsoft's App-V Client Cache. | None known. |
| %ProgramData%\Microsoft\Crypto | Cryptography. | None known. |
| %ProgramData%\Microsoft\DiagnosticLogCSP | Logging. | None known. |
| %ProgramData%\Microsoft\Microsoft Antimalware | Windows Defender. | None known. |
| %ProgramData%\Microsoft\Microsoft Security Client | Windows Defender. | None known. |
| %ProgramData%\Microsoft\EdgeUpdate | Microsoft Edge. | None known. |
| %ProgramData%\Microsoft\NetFramework\BreadcrumbStore | Unknown. | None known. |
| %ProgramData%\Microsoft\Search\Data | Windows Search. | None known. |
| %ProgramData%\Microsoft\Windows\Power Efficency Diagnostics | Power. | None known. |
| %ProgramData%\Microsoft\Windows\WER | Windows Error Reporting. | None known. |
| %ProgramData%\Microsoft\Windows Security Health | System monitoring. | None known. |
| %Programdata%\Package Cache | Unknown. | None known. |
| %ProgramData%\USOShared | Windows and One Drive. | None known. |
| %ProgramData%\USOPrivate | Windows and One Drive. | None known. |

## Public Documents area  (VFS\Common Documents)
| Entry | Explanation | Exceptions |
|----|----|----|
| C:\Users\Public\Documents\SequencedPackage | Installer logging for PassiveInstall. | None known. |

## User Profiles aka C:\Users (VFS\UserProfiles)
| Entry | Explanation | Exceptions |
|----|----|----|
| %UserProfiles% | Unclear | None known. |
| %UserProfiles%\AppData\Roaming\Microsoft\Crypto | Cryptography keys. | None known. |

## User Profile area (VFS\Profile)
| Entry | Explanation | Exceptions |
|----|----|----|
| %Profile%\Local Settings | Unknown. | None known. |
| %Profile%\NTUSER.DAT.Log1 | Registry. | None known. |
| %Profile%\NTUSER.DAT.Log2 | Registry. | None known. |

## User AppData\Local area  (VFS\LocalAppData)
| Entry | Explanation | Exceptions |
|----|----|----|
| %LocalAppData%\Microsoft\AppV | AppV Redirection. | None known. |
| %LocalAppData%\Microsoft\CLR_4.0\UsageLogs | C Language Runtime logs for x64 (or x86 on x86 system). | None known. |
| %LocalAppData%\Microsoft\CLR_4.0_32\UsageLogs | C Language Runtime logs for x86. | None known. |
| %LocalAppData%\Microsoft | Cryptography and more. | Care should be used in filtering this entire folder when repackaging Microsoft software. |
| %LocalAppData%\Microsoft Corporation | Logging. | None known. |
| %LocalAppData%\Microsoft OneDrive | OneDrive. | None known. |
| %LocalAppData%\Microsoft\Windows\AppRepository | Unknown. | None known. |
| %LocalAppData%\Microsoft\Windows\Documents | aka 'Personal'. | Some apps put documents down that are needed. |
| %LocalAppData%\Microsoft\Windows\History | activity. | None known. |
| %LocalAppData%\Microsoft\Windows\NetCache | temp files. | None known. |
| %LocalAppData%\Microsoft\Windows\NetCookies | Yum yum. | None known. |
| %LocalAppData%\Microsoft\Windows | Covers a lot of stuff.  Think it's OK though. | None known. |
| %LocalAppData%\Packages | UWP\MSIX package redirection area. | None known. |
| %LocalAppData%\SquirrelTemp | Unknown. | None known. |
| %LocalAppData%\Temp | User temp area. | None known. |

## User Program File area  (VFS\UserProgramFiles)
| Entry | Explanation | Exceptions |
|----|----|----|
| %LocalAppData%\Programs | User program installation area. Not really an issue, but you shouldn't be installing here. | None known. |

## User AppData\LocalLow area  (VFS\LocalAppDataLow)
| Entry | Explanation | Exceptions |
|----|----|----|
| %Profile%\Appdata\LocalLow\Microsoft\CryptnetUrlCache | Used by low integrity processes, like browsers. | None known. |

## User AppData\Roaming area  (VFS\AppData)
| Entry | Explanation | Exceptions |
|----|----|----|
| %AppData%\Microsoft\AppV | AppV Redirection. | None known. |
| %AppData%\Microsoft\Windows\Recent | Recent activity. | None known. |
| %AppData%\Microsoft\Windows\Themes | Windows Themes. Sometimes written to by background activity. | None known. |

## Windows area
| Entry | Explanation | Exceptions |
|----|----|----|
| C:\Windows\assembly\tmp | Temporary storage for DotNet. | None Known. |
| C:\Windows\Debug | Debugging. | None Known. |
| C:\Windows\INF\WmiApRpl\WmiApRpl.h | WMI/perfmon. | None Known. |
| C:\Windows\INF\WmiApRpl\WmiApRpl.ini | WMI/perfmon. | None Known. |
| C:\Windows\Installer | MSI caching. | Used for MSI self-repair, advertized shortcuts. Icons for shortcuts and fonts are often here too. Probably should not be a standard filter and intellegent manual cleanup should be performed. |
| C:\Windows\Microsoft.NET\Framework\v2.0.50727\ngen.log | NGEN Compilation log for x86 DotNet 2.* and 3.*. | None Known. |
| C:\Windows\Microsoft.NET\Framework\v4.0.30319\ngen.log | NGEN Compilation log for x86 DotNet 4.*. | None Known. |
| C:\Windows\Microsoft.NET\Framework64\v2.0.50727\ngen.log | NGEN Compilation log for x64 DotNet 2.* and 3.*. | None Known. |
| C:\Windows\Microsoft.NET\Framework64\v4.0.30319\ngen.log | NGEN Compilation log for x64 DotNet 4.*. | None Known. |
| C:\Windows\Logs | Windows logging. | None Known. |
| C:\Windows\Panther | Sysprep/OOBE. | None Known. |
| C:\Windows\Security | Windows unknown. | None Known. |
| C:\Windows\ServiceProfiles\NetworkService\AppData\Local\Microsoft\Windows\DeliveryOptimization | D.O. | None Known. |
| C:\Windows\ServiceProfiles\NetworkService\AppData\Local\Temp | Unknown. | None Known. |
| C:\Windows\servicing | Unknown. | None Known. |
| C:\Windows\System\config | Used when OS updates. | None known. | 
| C:\Windows\System\spp\store | Widnows system protection. | None known. | 
| C:\Windows\System32\config | Used when OS updates. | None known. | 
| C:\Windows\System32\perfc009.dat | WMI/perfmon. | None known. | 
| C:\Windows\System32\perfh009.dat | WMI/perfmon. | None known. | 
| C:\Windows\System32\PerfStringBackup.ini | WMI/perfmon. | None known. | 
| C:\Windows\System32\wbem\Performance\WmiApRpl.h | WMI/perfmon. | None known. | 
| C:\Windows\System32\wbem\Performance\WmiApRpl.ini | WMI/perfmon. | None known. | 
| C:\Windows\SysWow64\spp\store | Widnows system protection. | None known. | 
| C:\Windows\SysWow64\systemprofile\AppData\Local\Microsoft\CLR_v4.0\UsageLogs | C Language Runtime logs. | None known. | 
| C:\Windows\Temp | System Temporary files. | None Known. |
| C:\Windows\WinSxS\ManifestCache | DotNet manifest caching. | None Known. |
| C:\Windows\WindowsUpdate.log | WU. | None Known. |

## Native Program Files area (VFS\ProgramFilesX64)
| Entry | Explanation | Exceptions |
|----|----|----|
| C:\Program Files\Microsoft Security Client | Windows Defender. | None Known. |
| C:\Program Files\Windows Defender | Windows Defender. | None Known. |
| C:\Program Files\WindowsApps | UWP/MSIX packages. Background app updates. | None Known. |

## Off C: area (VFS\AppVPackageDrive)
| Entry | Explanation | Exceptions |
|----|----|----|
| C:\Config.msi | Some unpacked MSIs are written here by exe installers. | None Known. |
| C:\$Recycle.Bin | Deleted files. | None Known. |
| C:\System Volume Information | NTFS File System area. | None Known. |

## General (places like the Desktops)
| Entry | Explanation | Exceptions |
|----|----|----|
| *\Desktop.ini | Appears in many folders. | None Known. |
