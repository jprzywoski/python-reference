====
seek
====

Description
===========
Sets the file’s current position.

Syntax
======
**file**. *seek(offset[, whence])*

*offset*
    Required. The *offset* from the beginning of the file.
*whence*
    Optional. The *whence* argument is optional and defaults to *os.SEEK_SET* or 0 (absolute file positioning); other values are *os.SEEK_CUR* or 1 (seek relative to the current position) and *os.SEEK_END* or 2 (seek relative to the file’s end). There is no return value.

Remarks
=======
Note that if the file is opened for appending (mode *'a'* or *'a+'*), any *seek()* operations will be undone at the next write. If the file is only opened for writing in append mode (mode *'a'*), this method is essentially a no-op, but it remains useful for files opened in append mode with reading enabled (mode *'a+'*). If the file is opened in text mode (without *'b'*), only offsets returned by *tell()* are legal. Use of other offsets causes undefined behavior.

Note that not all file objects are seekable.

Changed in version 2.6: Passing float values as offset has been deprecated.

Return Value
============
**None**

Time Complexity
===============
#TODO

Example 1
=========
>>> # test.txt contents:
>>> # ABCDE
>>> f = open(r'C:\test.txt')
>>> f.seek(3)
>>> f.read()   # starts reading from the 3rd character
'DE'

Example 2
=========
>>> f = open(r'C:\test.txt')
>>> f.seek(2)    # move two characters ahead
>>> f.seek(2, 1) # move two characters ahead from the current position
>>> f.read()
'E'

Example 3
=========
>>> f = open(r'C:\test.txt')
>>> f.seek(-3, 2) # move to the 3rd character from the end of the file
>>> f.read()
'CDE'

See Also
========
#TODO

