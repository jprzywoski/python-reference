====
file
====

Description
===========
Returns a file object.

Syntax
======
**file** *(name[, mode[, buffering]])*

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
*buffering*
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

Note
====
When opening a file, it’s preferable to use open() instead of invoking this constructor directly. file is more suited to type testing (for example, writing isinstance(f, file)).

Example
=======
>>> file('C:\\alice_in_wonderland.txt')
<open file 'C:\\alice_in_wonderland.txt', mode 'r' at 0x02C1C390>
>>> alice = open(r'C:\alice_in_wonderland.txt', 'r+')
>>> alice.readline()
"                ALICE'S ADVENTURES IN WONDERLAND\n"

See Also
========
#TODO