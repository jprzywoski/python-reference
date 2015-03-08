==========
writelines
==========

Description
===========
Writes a sequence of strings to the file.

Syntax
======
**file**. *writelines(iterable)*

*sequence*
    Any iterable object producing strings, typically a list of strings.

Remarks
=======
There is no return value. (The name is intended to match *readlines()*; *writelines()* does not add line separators.)
Files support the iterator protocol. Each iteration returns the same result as *readline()*, and iteration ends when the *readline()* method returns an empty string.

File objects also offer a number of other interesting attributes. These are not required for file-like objects, but should be implemented if they make sense for the particular object.

Return Value
============
**None**

Time Complexity
===============
#TODO

Example
=======
>>> f = open(r'C:\test.txt', 'w')
>>> f.writelines(['foo', 'bar'])
>>> f.close()
>>> f = open(r'C:\test.txt')
>>> f.read()
'foobar'

See Also
========
#TODO
