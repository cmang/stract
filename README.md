## Stract

Stract tries to make it simple to extract a range of bytes from a file and save it as a new file.

It is useful for CTFs, for extracting files from ROM, disk and memory images, extracting hashes and certificates from binaries, and many other things. It is much faster than "binwalk" for extracting individual files. The Unix utility "dd" does the heavy lifting, so it should work on any Unix or Linux system.

## Requirements

Python 3.x

It should work in Windows if you have "dd" installed and in the path.

## Usage:

    stract inputfile outputfile firstbye [lastbyte]

"firstbyte" and "lastbyte" offsets can be in decimal or hex format. Prefix with 0x for hexadecimal. Omit "lastbyte" to extract until the end of the file.

## Legal:

BSD 3-Clause License, see LICENSE file for details.

Copyright (c) 2022, Sam Foster
All rights reserved.

