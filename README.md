# AHKv2-Gdip
This repository contains the GDI+ library (Gdip_All.ahk) compatible with [AHK v2-a081](https://autohotkey.com/v2/) and also backwards compatible with AHK v1.1.26.01  

AHK v2 made many changes to the syntax, which is why changes were needed. We have attempted to keep it backwards compatible with AHK v1.1 as much as possible. If you find any errors please report them in the Issues.  

Support for AHK v1.0 is dropped (find the original `Gdip_All.ahk` library if you need that).  

See the [commit history](https://github.com/mmikeww/AHKv2-Gdip/commits/master) to see the changes made. There is probably lots of room for improvement still.  

# Examples
All of the tutorial files in the `/Examples/` subfolder work successfully on AHK v2.  

If you try to run these example files on AHK v1, they will fail. However, the v1 code is still in the files, and simply commented out. Search the example files for "AHK v1" and swap the commented lines to get them working.  

# Usage
All of the Gdip_*() functions use the same syntax as before, so no changes should be required.  

The one exception is for `Gdip_BitmapFromBRA()`. It requires you to read the .bra file witih `FileObj.RawRead()` instead of the `FileRead`command. See the Tutorial.11 file in the Examples folder  

# History
- @tic created the original [Gdip.ahk](https://github.com/tariqporter/Gdip/) library
- @Rseding91 updated it to make it compatible with unicode and x64 AHK versions and renamed the file `Gdip_All.ahk`
- this repository updates @Rseding91's `Gdip_All.ahk` to make it compatible with AHK v2

