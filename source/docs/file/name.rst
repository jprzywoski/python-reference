====
name
====

Description
===========
Returns the name of the file.

Syntax
======
**file**. *name*

Remarks
=======
If the file object was created using *open()*, the name of the file. Otherwise, some string that indicates the source of the file object, of the form <...>. This is a read-only attribute and may not be present on all file-like objects.

Return Value
============
**None**

Time Complexity
===============
#TODO

Example
=======
>>> f = open(r'C:\test.txt')
>>> f.name
'C:\\test.txt'

See Also
========
#TODO
