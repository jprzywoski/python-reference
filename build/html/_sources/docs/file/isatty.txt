======
isatty
======

Description
===========
Returns True if the file is if the stream is interactive (i.e., connected to a terminal/tty device).

Syntax
======
**file**. *isatty()* 

Note
====
If a file-like object is not associated with a real file, this method should not be implemented.

Return Value
============
**None**

Time Complexity
===============
#TODO

Example
=======
>>> f = open(r'C:\aiw.txt')
>>> f.isatty()
False

See Also
========
#TODO
