====
read
====

Description
===========
Returns specified amount of bytes from the file.

Syntax
======
**file**. *read([size])*

*size*
    Optional. Reads at most *size* bytes from the file (less if the read hits *EOF* before obtaining size bytes). If the size argument is negative or omitted, reads all data until EOF is reached.

Remarks
=======
The bytes are returned as a string object. An empty string is returned when *EOF* is encountered immediately. (For certain files, like ttys, it makes sense to continue reading after an *EOF* is hit.)

Note that this method may call the underlying C function *fread()* more than once in an effort to acquire as close to size bytes as possible. Also note that when in non-blocking mode, less data than was requested may be returned, even if no size parameter was given.

Note
====
This function is simply a wrapper for the underlying *fread()* C function, and will behave the same in corner cases, such as whether the *EOF* value is cached.

Return Value
============
**None**

Time Complexity
===============
#TODO

Example
=======
>>> f.read(8)
'        '
>>> f.read(128)
"        ALICE'S ADVENTURES IN WONDERLAND\n\n                          Lewis Carroll\n\n               THE MILLENNIUM FULCRUM EDITION"
>>> f.read() # this returns contents of the whole file

See Also
========
#TODO
