======
fileno
======

Description
===========
Returns the integer *file descriptor*.

Syntax
======
**file**. *fileno()*

Remarks
=======
The integer *file descriptor* is used by the underlying implementation to request I/O operations from the operating system. This can be useful for other, lower level interfaces that use file descriptors, such as the *fcntl* module or *os.read()* and friends.

Note
====
File-like objects which do not have a real file descriptor should not provide this method!

Return Value
============
**None**

Time Complexity
===============
#TODO

Example
=======
>>> f = open(r'C:\aiw.txt')
>>> f.fileno()
3
>>> f1 = open(r'C:\aiw.txt')
>>> f1.fileno()
4

See Also
========
#TODO
