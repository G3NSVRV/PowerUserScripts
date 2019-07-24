# Normalize (fix) Folder Permissions in Linux

This script was maded to fix the folder permissions on Linux for Windows 10 (WSL) which by default leaves every file/folder with permission 777, which is not recommended at all.

This also works for any flavor of Linux.

## Usage:
```
./fixPermissions $FOLDER_PATH
```
or
```
./fixPermissions
(which will read the current work path; $PWD)
```
