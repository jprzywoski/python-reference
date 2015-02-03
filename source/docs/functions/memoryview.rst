==========
memoryview
==========

Description
===========
Returns a memoryview object.

Syntax
======
**memoryview** *(object)*

*object*
	Required. An object supporting buffer protocol - str and bytearray (but not unicode).

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
The memoryview() function allows direct read and write access to an object's byte-oriented data without needing to copy it first. That can yield large performance gains when operating on large objects since it doesn’t create a copy when slicing.
See also buffer().

Example
=======
>>> memoryview('foo')
<memory at 0x02CCCDA0>
>>> m = memoryview('foo')
>>> m[:]
<memory at 0x02CCCF80>
>>> m[1]
'o'

See Also
========
#TODO
