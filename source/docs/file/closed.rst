======
closed
======

Description
===========
Returns a Boolean stating whether the file is closed.

Syntax
======
**file**. *closed*

Remarks
=======
This is a read-only attribute; the *file.close()* method changes the value. It may not be available on all file-like objects.

Example
=======
>>> f = open(r'C:\test.txt')
>>> f.closed
False
>>> f.close()
>>> f.closed
True