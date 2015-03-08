=========
softspace
=========

Description
===========
Returns a Boolean that indicates whether a space character needs to be printed before another value when using the print statement.

Syntax
======
**file**. *softspace*

Remarks
=======
Classes that are trying to simulate a file object should also have a writable softspace attribute, which should be initialized to zero. This will be automatic for most classes implemented in Python (care may be needed for objects that override attribute access); types implemented in C will have to provide a writable softspace attribute.

Note
====
This attribute is not used to control the print statement, but to allow the implementation of print to keep track of its internal state.

Return Value
============
**None**

Time Complexity
===============
#TODO

Example
=======
>>> f = open(r'C:\test.txt')
>>> f.softspace
0

See Also
========
#TODO
