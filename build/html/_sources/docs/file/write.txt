=====
write
=====

Description
===========
Writes a string to the file.

Syntax
======
**file**. *write(str)*

*str*
    A string you want to write to the file.

Remarks
=======
There is no return value. Due to buffering, the string may not actually show up in the file until the *flush()* or *close()* method is called.

Return Value
============
**None**

Time Complexity
===============
#TODO

Example
=======
>>> f = open(r'C:\test.txt', 'w')
>>> f.write('foo')
>>> f.close()
>>> f = open(r'C:\test.txt')
>>> f.read()
'foo'

See Also
========
#TODO
