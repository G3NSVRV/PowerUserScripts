# Restore ACLs on "C:\Program Files\WindowsApps" Folder Windows 10

This scripts restores all the ACLs (permissions) on "C:\Program Files\WindowsApps" Folder (UWP apps) automatically without any mayor user intervention using any Bash for Windows 10 ([e.g. Ubuntu](https://www.microsoft.com/store/productId/9NBLGGH4MSV6)).

## Things to Consider before to run this script
This script was designed to be used on Windows 10.
It uses the default SID capability to work with UWP which is:

*(From Windows 8 and above)*

`S-1-15-3-1024-1065365936-1281604716-3511738428-1654721687-432734479-3232135806-4053264122-3456934681`

If you found and or feel that your SID is different, please replace it on the **template.acl** file

You can read for more information [on this site](https://support.microsoft.com/en-us/help/4502539/some-sids-do-not-resolve-into-friendly-names)
## Usage
The script will automatically change the owner of the folder "C:\Program Files\WindowsApps" using the group "Administrators", then it will apply the ACL and return to the owner "NT Service\TrustedInstaller".

```
$: ./restoreAcls
