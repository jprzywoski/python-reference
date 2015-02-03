========
readline
========

Description
===========
Reads one entire line from the file.

Syntax
======
**file**. *readline([size])*

*size*
    Optional. If the size argument is present and non-negative, it is a maximum byte count (including the trailing newline) and an incomplete line may be returned. When size is not 0, an empty string is returned only when *EOF* is encountered immediately.

Remarks
=======
A trailing newline character is kept in the string (but may be absent when a file ends with an incomplete line). 

Note
====
Unlike stdio‘s *fgets()*, the returned string contains null characters ('\0') if they occurred in the input.

Example
=======
>>> f = open(r'C:\aiw.txt')
>>> f.readline()
"                ALICE'S ADVENTURES IN WONDERLAND\n"
>>> f.readline(32)
'\n'
>>> f.readline(64)
'                          Lewis Carroll\n' 