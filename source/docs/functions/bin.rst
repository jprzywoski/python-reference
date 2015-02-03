===
bin
===

Description
===========
Returns an integer converted into a binary string.

Syntax
======
**bin** *(integer)*

*integer*
	Required. An integer value to be converted into binary string.

Return Value
============
**str**

Time Complexity
===============
#TODO

Note
====
If number is not a Python int object, it has to define an __index__() method that returns an integer.

Example
=======
>>> bin(1)
'0b1'
>>> bin(1024)
'0b10000000000'
>>> bin(0b0111 + 0b1000)
'0b1111'

See Also
========
#TODO

