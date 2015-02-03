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
Sets the file’s current position, like stdio‘s *fseek()*. 

Note that if the file is opened for appending (mode *'a'* or *'a+'*), any *seek()* operations will be undone at the next write. If the file is only opened for writing in append mode (mode *'a'*), this method is essentially a no-op, but it remains useful for files opened in append mode with reading enabled (mode *'a+'*). If the file is opened in text mode (without *'b'*), only offsets returned by *tell()* are legal. Use of other offsets causes undefined behavior.

Note that not all file objects are seekable.
Changed in version 2.6: Passing float values as offset has been deprecated.

Example 1
=========
>>> # test.txt contents:
>>> # foobar snafu
>>> f = open(r'C:\test.txt')
>>> f.seek(3)
>>> f.read()   # starts reading from the 3rd character
'bar snafu'

Example 2
=========
>>> f = open(r'C:\test.txt')
>>> f.seek(2)
>>> f.seek(2, 1) # advances the current position by two
>>> f.read()
'ar snafu'

Example 3
=========
>>> f = open(r'C:\test.txt')
>>> f.seek(-3, 2) # sets the position to the third to last
>>> f.read()
'afu' 

