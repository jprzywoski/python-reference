====
mode
====

Description
===========
Returns the I/O mode for the file.

Syntax
======
**file**. *mode*

Remarks
=======
If the file was created using the *open()* built-in function, mode will be the value of the mode parameter. This is a read-only attribute and may not be present on all file-like objects.

Example
=======
>>> f = open(r'C:\test.txt', 'w')
>>> f.mode
'w' 