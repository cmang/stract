Stract

Stract tries to make it simple to extract a range of bytes from a file and save it as a new file.

syntax:

    stract <inputfile> <outputfile> <firstbye> <lastbyte>

"firstbyte" and "lastbyte" offsets can be in decimal or hex format. Prefix with 0x for hexadecimal.

This program requires the program "dd" which should be preinstalled on any Unix or Linux system.
It should work in Windows if you have "dd" installed and in the path.

It also requires Python 3.

It is useful for CTFs, for extracting files from ROM images, etc. It is much faster than "binwalk" for extracting individual files.

Credits: Sam Foster, 2022

License: See LICENSE file

