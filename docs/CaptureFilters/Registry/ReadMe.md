# Capture Filters: Registry

This is the folder for information on setting up application capture filters for Registry keys and items.

It is important not only to document the items we typically want cleaned out of repackaging efforts, but to:

* `Entry`: Document what the thing(s) is/are being removed.
* `Explanation`: What is is/Why it isn't needed.
* `Exceptions`: Any special situations where it should not be removed.

The information provided assumes packaging on x64 systems.

## HKLM  (REGISTRY\MACHINE)
| Entry | Explanation | Exceptions |
|----|----|----|
| Components | Unknown | None known. |
| SOFTWARE\Microsoft\AppV | App-V. | None known. |
| SOFTWARE\Microsoft\Cryptography | Cryptography. | None known. |
| SOFTWARE\Microsoft\Microsoft Antimalware | Windows Defender. | None known. |
| SOFTWARE\Microsoft\Microsoft Antimalware Setup | Windows Defender. | None known. |
| SOFTWARE\Microsoft Security Center | Security. | None known. |
| SOFTWARE\Microsoft\WBEM | WMI. | Compiled MOFs for WMI Providers. |
| SOFTWARE\Microsoft\Windows\CurrentVersion\AUTHENTICATION | Authentication. | None known. |
| SOFTWARE\Microsoft\Windows\CurrentVersion\Census | Unknown. | None known. |
| SOFTWARE\Microsoft\Windows\CurrentVersion\COMPONENT BASED SERVICING | OS Updating. | None known. |
| SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\GlobalAssocChangedCounter | Windows File explorer. | None known. |
| SOFTWARE\Microsoft\Windows\CurrentVersion\OneSettings | Unknown. | None known. |
| SOFTWARE\Microsoft\Windows\CurrentVersion\Setup | OS Updating. | None known. |
| SOFTWARE\Microsoft\Windows\CurrentVersion\Uninstall | uninstalling. | None known. |
| SOFTWARE\Microsoft\Windows\CurrentVersion\WindowsUpdate | Happens when WU turns back on again. | None known. |
| SOFTWARE\Microsoft\Windows\CurrentVersion\Wosc | Unknown. | None known. |
| SOFTWARE\Microsoft\Windows Defender | Unknown. | None known. |
| SOFTWARE\Microsoft\Windows NT\CurrentVersion\Notifications | Unknown. | None known. |
| SOFTWARE\Microsoft\Windows NT\CurrentVersion\Perflib | WMI. | None known. |
| SOFTWARE\Microsoft\Windows NT\CurrentVersion\SoftwareProtectionPlatform | spp. | None known. |
| SOFTWARE\Microsoft\Windows NT\CurrentVersion\SystemRestore | Not needed in repackaging. | None known. |
| SOFTWARE\Microsoft\WindowsUpdate | Happens when WU turns back on again. | None known. |
| SOFTWARE\Microsoft\Policies\Microsoft\Microsoft Antimalware | Windows Defender. | None known. |
| SOFTWARE\Microsoft\Policies\Microsoft\Windows Defender | Windows Defender. | None known. |
| SOFTWARE\Wow6432Node\Microsoft\AppV | App-V. | None known. |
| SOFTWARE\Wow6432Node\Microsoft\Cryptography | Cryptography. | None known. |
| SOFTWARE\Wow6432Node\Microsoft\DownloadManager | Updates. | None known. |
| SOFTWARE\Wow6432Node\Microsoft\EdgeUpdate | Microsoft Edge. | None known. |
| SOFTWARE\Wow6432Node\Microsoft\Explorer\GlobalAssocChangedCounter | Windows File explorer. | None known. |
| SOFTWARE\Wow6432Node\Microsoft\Tracing | Logs. | None known. |
| SYSTEM\CurrentControlSet\Control\CloudDomainJoin | Azure. | None known. |
| SYSTEM\CurrentControlSet\Control\Cryptography | Cryptography. | None known. |
| SYSTEM\CurrentControlSet\Control\MUI | Unknown, but likely language. | None known. |
| SYSTEM\CurrentControlSet\Control\Session Manager | Unknown. | None known. |
| SYSTEM\CurrentControlSet\Control\WMI | WMI. | None known. |
| SYSTEM\CurrentControlSet\Services\bam | Bitlocker. | None known. |
| SYSTEM\CurrentControlSet\Services\BITS | SCCM Download and run. | None known. |
| SYSTEM\CurrentControlSet\Services\TrustedInstaller | UWP/MSIX. | None known. |
| SYSTEM\CurrentControlSet\Services\VSS | Volume Shaddow Service. | None known. |
| SYSTEM\CurrentControlSet\Services\WdBoot | Windows Defender. | None known. |
| SYSTEM\CurrentControlSet\Services\WdFilter | Windows Defender. | None known. |
| SYSTEM\CurrentControlSet\Services\WdNisDrv | Windows Defender. | None known. |
| SYSTEM\CurrentControlSet\Services\WdNisSvc | Windows Defender. | None known. |
| SYSTEM\CurrentControlSet\Services\WinDefend | Windows Defender. | None known. |
| SYSTEM\CurrentControlSet\Services\WmiApRpl | WMI. | None known. |
| SYSTEM\CurrentControlSet\WaaS | Windows Updates. | None known. |


## Default Users hive (REGISTRY\USER\.Default)
| Entry | Explanation | Exceptions |
|----|----|----|
| Software\CLASSES\LOCAL SETTINGS\MUICACHE | Language | None known. |
| Software\Microsoft\IdentityCRL | Unknown. | None known. |
| Software\Microsoft\Windows\CurrentVersion\Explorer\Accent | Windows File Explorer Unknown. | None known. |
| Software\Microsoft\Windows\CurrentVersion\Themes | Windows. | None known. |
| Software\Microsoft\Windows\DWM | Desktop Window Manager. | None known. |


## HKCU (REGISTRY\USER\[{AppVCurrentUserSID}])
| Entry | Explanation | Exceptions |
|----|----|----|
| Classes\AppID\OneDrive.EXE | One Drive. | None known. |
| Classes\OOBERequestHandler | Windows OOBE. | None known. |
| Classes\SyncEngineFileInfoProvider | Unknown. | None known. |
| Software\Microsoft\AppV | Microsoft App-V. | None known. |
| Software\Microsoft\CTF | Unknown. | None known. |
| Software\Microsoft\IdentityCRL | Unknown. | None known. |
| Software\Microsoft\OneDrive | One Drive. | None known. |
| Software\Microsoft\RestartManager | OS Restarts. | None known. |
| Software\Microsoft\Speech_OneCore | Speach to text. | None known. |
| Software\Microsoft\Windows\CurrentVersion\CloudStore | Microsoft Store. | None known. |
| Software\Microsoft\Windows\CurrentVersion\ContentDeliveryManager | Updates. | None known. |
| Software\Microsoft\Windows\CurrentVersion\Explorer\FeatureUsage |  Windows File Explorer. | None known. |
| Software\Microsoft\Windows\CurrentVersion\Explorer\FileExts\.ps1\OpenWithList\MRUList | When FTA is used to launch a script. | None known. |
| Software\Microsoft\Windows\CurrentVersion\Explorer\FileExts\.ps1\OpenWithProgIDs | When FTA is used to launch a script. | . | None known. |
| Software\Microsoft\Windows\CurrentVersion\Explorer\RecentDocs | Windows File Explorer. | None known. |
| Software\Microsoft\Windows\CurrentVersion\Explorer\SessionInfo | Windows File Explorer. | None known. |
| Software\Microsoft\Windows\CurrentVersion\Explorer\SlowContextMenuEntries | Windows File Explorer. | None known. |
| Software\Microsoft\Windows\CurrentVersion\Explorer\Streams |  Windows File Explorer. | None known. |
| Software\Microsoft\Windows\CurrentVersion\Explorer\UserAssist | Windows File Explorer. | None known. |
| Software\Microsoft\Windows\CurrentVersion\Explorer\Wow3264Node\StreamMRU |  Windows File Explorer. | None known. |
| Software\Microsoft\Windows\CurrentVersion\Feeds | Unknown. RSS? | None known. |
| Software\Microsoft\Windows\CurrentVersion\Internet Settings\5.0\Cache | Browser. | None known. |
| Software\Microsoft\Windows\CurrentVersion\Internet Settings\ZoneMap | Browser. | None known. |
| Software\Microsoft\Windows\CurrentVersion\Search | Search. | None known. |
| Software\Microsoft\Windows\CurrentVersion\Security and Maintenance | Unknown. | None known. |
| Software\Microsoft\Windows\CurrentVersion\Shell Extensions\Cached | Windows File Explorer. | None known. |
| Software\Microsoft\Windows\CurrentVersion\SessionInfo | Unknown. | None known. |
| Software\Microsoft\Windows\CurrentVersion\UFH | Unknown. | None known. |
| Software\Microsoft\Windows\Shell\Bags | Windows File Explorer. | None known. |
| Software\Microsoft\Windows\Shell\BagMRU | Windows File Explorer. | None known. |
| Software\Microsoft\Windows NT\CurrentVersion\Winlogon\PUUActive | Unknown. | None known. |



## HK System User (REGISTRY\USER\S-1-5-20)
| Entry | Explanation | Exceptions |
|----|----|----|
| Software\Microsoft\Speech_OneCore | Unknown. | None known. |
| Software\Microsoft\Windows\CurrentVersion\DeliveryOptimization | Unknown. Possibly D.O. for 'PreProvisioned' Apps. | None known. |
