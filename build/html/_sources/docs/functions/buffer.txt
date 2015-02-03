======
buffer
======

Description
===========
Returns a new buffer object which references the object argument.

Syntax
======
**buffer** *(object[, offset[, size]])*

*object*
	Required. The object argument must be an object that supports the buffer call interface (such as string, unicode, bytearray, mmap.mmap or array.array).
*offset*
	Optional. Buffer slice offset; if omitted the buffer object will be a slice from the beginning of object.
*size*
	Optional. Length of the slice; if omitted the slice will extend to the end of object.

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
The buffer() function allows direct (read-only) access to an object's byte-oriented data without needing to copy it first. That can yield large performance gains when operating on large objects since it does not create a copy of an object when slicing.
See memoryview() for read and write access.

Example
=======
>>> b = buffer('hello')
>>> b
<read-only buffer for 0x00EE38A0, size -1, offset 0 at 0x00EE3020>
>>> print b
hello
>>> b = buffer('hello', 1)
>>> print b
ello
>>> b = buffer('hello', 1, 3)
>>> print b
ell

See Also
========
#TODO