# WARNING

This is a hacky, modified, version of the NTFS-3g (based on ntfs-3g_ntfsprogs-2016.2.22)
driver that allows mounting a NTFS filesystem with its NTFS Master File Table (MFT)
corrupted, meaning that the MFT and the MFTMirror do not match. Such missmatch makes
Windows happily ask you if you want to format your drive because it is "unreadable".

See https://en.wikipedia.org/wiki/NTFS#Master_File_Table for some information
about the NTFS's MFT.

Folder `patches/` contains the relevant (and irrelevant) changes performed while
hacking around the code.

Hope this will save someone's life as it saved mine :D
