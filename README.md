Copy Contents to Clipboard Version 1.0.0
====
Section 1: About:
This Registry file adds a context menu entry to various text-based files. Right-clicking on one of these files and choosing 'Copy Contents to Clipboard' will put the contents of that file into the clipboard, without having to open an application and manually selecting the data. The currently supported filetypes are:
.txt
.rtf
.csv
.ini
.reg
See Section 3 for information about adding more filetypes.

Section 2: Usage and Installation:
To Install, simply double-click the included fileToClipboard.reg file. No Reboot is required.
To Use, right-click on a supported file type and choose 'Copy Contents to Clipboard'.

Section 3: Extensibility
You can add additional filetypes to the supported list, as long as that file stores data as text, such as .bat files, .vbs files, or .html files.
To add a file type, you need to first determine the file handler in the registry.
1) Open the Registry Editor (start -> run -> regedit)
2) Browse the HKEY_Classes_Root tree until you find the file extenstion you wish to add, or press f3 to search.
3) Click on the key for that extension. The 'Default' field will have an entry in it, such as txtfile or batfile. Copy the contents of that entry.
4) Make a copy of the AddFileType.reg file, and rename this copy to something you recognize.
5) Right-click your new file, and choose edit.
6) Replace the instances 'filetype' in your new file with the handler you copied from the registry editor earlier in step 3.
7) Save your changes to your new file.
8) Double click your new file, and add the entries to the registry. Your new file type is now supported, and can you can copy its contents to the clipboard.

