## Stract

Stract tries to make it simple to extract a range of bytes from a file and save it as a new file.

It is useful for CTFs, for extracting files from ROM, disk and memory images, extracting hashes and certificates from binaries, and many other things. It is much faster than "binwalk" for extracting individual files and data from very large files.

## Requirements

Python 3.x

## Usage:

    stract inputfile outputfile firstbye [lastbyte]

Examples:

    $ stract logo.gif extracted.txt 0x00000048 0x00000052
    Extracting bytes 72 to 82 (11 bytes total) from logo.gif...
    Wrote to file: extracted


"firstbyte" and "lastbyte" offsets can be in decimal or hexadecimal format. Prefix with 0x for hexadecimal. Omit "lastbyte" to extract until the end of the file.

You can find interesting offsets to use by examining binary files in a hex editor, or with an automated tool like binwalk.

## Legal:

BSD 3-Clause License, see LICENSE file for details.

Copyright (c) 2022, Sam Foster
All rights reserved.

