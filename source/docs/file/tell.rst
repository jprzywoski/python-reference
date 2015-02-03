====
tell
====

======

Description
===========
Returns the file’s current position.

Syntax
======
**file**. *tell()*

Remarks
=======
Works like stdio‘s *ftell()*.

Note
====
On Windows, *tell()* can return illegal values (after an *fgets()*) when reading files with Unix-style line-endings. Use binary mode (*'rb'*) to circumvent this problem.

Example
=======
>>> # test.txt contents:
>>> # foobar snafu
>>> f = open(r'C:\test.txt')
>>> f.tell()
0L
>>> f.seek(3)  # changes position by 3
>>> f.tell()
3L 