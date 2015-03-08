========
truncate
========

Description
===========
Truncates the file’s size.

Syntax
======
**file**. *truncate([size])*

*size*
    Optional. If the optional *size* argument is present, the file is truncated to (at most) that size. The size defaults to the current position.

Remarks
=======
The current file position is not changed.

Note that if a specified size exceeds the file’s current size, the result is platform-dependent: possibilities include that the file may remain unchanged, increase to the specified size as if zero-filled, or increase to the specified size with undefined new content. Availability: Windows, many Unix variants.

Return Value
============
**None**

Time Complexity
===============
#TODO

Example
=======
>>> # test.txt contents:
>>> # ABCDE
>>> f = open(r'C:\test.txt', 'r+')
>>> f.truncate(2)
>>> f.read()
'AB'

See Also
========
#TODO
