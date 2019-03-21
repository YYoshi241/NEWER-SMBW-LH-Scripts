# NEWER-SMBW-LH-Scripts
Scripts and Tools necessary to prepare Newer SMBW Wii for Reggie Next


Instructions

NEWER_LH_DECOMPRESS.bat

Run this script inside of the NewerSMBW folder of your copy of Newer Super Mario Bros. Wii.
It will output all LH compressed files in the Subdirectories of this folder. (File names are directly specified to a unmodified Newer 1.2.0)


REGGIE_NEXT_TILESET_FIX.bat

Run this script to fix the "tileset X.arc is not found" error.
IT copies the ARC files from /Tilesets to /Stages/Texture/

ntcompress.exe

Tool that makes the scripts work. This tool can (de)compress serveral Wii file types. 
This file only exists here so you don't have to find it online yourself.
(NOTE: This can also be found easily on the internet if you search "NewerSMBW editor" or similar)

What about RE-compressing files.

I haven't figured out a way (yet) to easily make a (re)compresion script for the extracted files for ntcompress.
so you'll have to manually compress the files you've edited yourself.

ntcompress -lh <filename or path including file name ie. 01-01.arc or /Stages/01-01.arc>

then rename the file to <original file name ie. 01-01.arc>.LH as it will ouput the file with "_LH.bin" at the end.

How to help this repository.

Add issues about faults in uploaded scripts, and place pull-requests for new or updated scripts to add to this repository (especially for the LH (re)compression script.)

Notes:                   
All of the current scripts (and the Tool that powers them) are Windows ONLY. If ntcompress and/or the scripts can be ran on Linux or macOS using something like Wine, please post an Issue mentioning that so I can update the README.
