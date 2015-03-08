====
tell
====

Description
===========
Returns the file’s current position.

Syntax
======
**file**. *tell()*

Note
====
On Windows, *tell()* can return illegal values (after an *fgets()*) when reading files with Unix-style line-endings. Use binary mode (*'rb'*) to circumvent this problem.

Return Value
============
**long**

Time Complexity
===============
#TODO

Example
=======
>>> # test.txt contents:
>>> # 0000 0000
>>> f = open(r'C:\test.txt')
>>> f.tell()
0L
>>> f.seek(3)  # changes position by 3
>>> f.tell()
3L

See Also
========
#TODO
