=========
readlines 
=========

Description
===========
Returns a list containing lines from the file.

Syntax
======
**file**. *readlines([sizehint])*
 
*sizehint*
    Optional. If the optional *sizehint* argument is present, instead of reading up to *EOF*, whole lines totalling approximately *sizehint* bytes (possibly after rounding up to an internal buffer size) are read.

Remarks
=======
Reads lines until *EOF* using *readline()* and return a list containing the lines thus read. Objects implementing a file-like interface may choose to ignore *sizehint* if it cannot be implemented, or cannot be implemented efficiently.

Return Value
============
**list**

Time Complexity
===============
#TODO

Example
=======
>>> f = open(r'C:\aiw.txt')
>>> f.readlines()  # this will return the list of all the lines in the file

See Also
========
#TODO
