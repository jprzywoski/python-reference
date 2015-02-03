====
open
====

Description
===========
Opens a file returning a file object.

Syntax
======
**open** *(name[, mode[, buffering]])*

*name*
	Optional. Full filepath.
*mode*
	Optional. Possible values:
    'r' open for reading (default)
    'w' open for writing, truncating the file first
    'a' open for writing, appending to the end of the file if it exists
    'b' binary mode
    't' text mode (default)
    '+' open a disk file for updating (reading and writing)
    'U' universal newlines mode (for backwards compatibility; should not be used in new code)
buffering*
	Optional. Possible values:
    ‘0’ to switch buffering off (only allowed in binary mode)
    ‘1’ to select line buffering (only usable in text mode)
    ‘integer > 1’ to indicate the size of a fixed-size chunk buffer

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
The most commonly-used values of mode are 'r' for reading, 'w' for writing (truncating the file if it already exists), and 'a' for appending (which on some Unix systems means that all writes append to the end of the file regardless of the current seek position). If mode is omitted, it defaults to 'r'. The default is to use text mode, which may convert '\n' characters to a platform-specific representation on writing and back on reading. Thus, when opening a binary file, you should append 'b' to the mode value to open the file in binary mode, which will improve portability. (Appending 'b' is useful even on systems that don’t treat binary and text files differently, where it serves as documentation.) See below for more possible values of mode.

The optional buffering argument specifies the file’s desired buffer size: 0 means unbuffered, 1 means line buffered, any other positive value means use a buffer of (approximately) that size (in bytes). A negative buffering means to use the system default, which is usually line buffered for tty devices and fully buffered for other files. If omitted, the system default is used.

Modes 'r+', 'w+' and 'a+' open the file for updating (note that 'w+' truncates the file). Append 'b' to the mode to open the file in binary mode, on systems that differentiate between binary and text files; on systems that don’t have this distinction, adding the 'b' has no effect.

In addition to the standard fopen() values mode may be 'U' or 'rU'. Python is usually built with universal newlines support; supplying 'U' opens the file as a text file, but lines may be terminated by any of the following: the Unix end-of-line convention '\n', the Macintosh convention '\r', or the Windows convention '\r\n'. All of these external representations are seen as '\n' by the Python program. If Python is built without universal newlines support a mode with 'U' is the same as normal text mode. Note that file objects so opened also have an attribute called newlines which has a value of None (if no newlines have yet been seen), '\n', '\r', '\r\n', or a tuple containing all the newline types seen.

Python enforces that the mode, after stripping 'U', begins with 'r', 'w' or 'a'.

Python provides many file handling modules including fileinput, os, os.path, tempfile, and shutil.

Example
=======
>>> open('C:\\alice_in_wonderland.txt')
<open file 'C:\\alice_in_wonderland.txt', mode 'r' at 0x02C1C390>
>>> alice = open(r'C:\alice_in_wonderland.txt', 'r+')
>>> alice.readline()
"                ALICE'S ADVENTURES IN WONDERLAND\n"

See Also
========
#TODO