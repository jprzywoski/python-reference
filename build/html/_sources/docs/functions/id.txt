==
id
==

Description
===========
Returns the “identity” of an object.

Syntax
======
**id** *(object)*

*object*
	Required. An object which id is to be returned.

Return Value
============
#TODO

Time Complexity
============
#TODO

Note
====
CPython implementation detail: This is the address of the object in memory.

Remarks
=======
This is an integer (or long integer) which is guaranteed to be unique and constant for this object during its lifetime.
Two objects with non-overlapping lifetimes may have the same id() value.

Example
=======
>>> l1 = [1, 2]
>>> l2 = [1, 2]
>>> id(l1)
46449768
>>> id(l2)
46210984
>>> id(l1) == id(l2)# note that objects with the same value can have different ids
False
>>> l1 == l2
True

See Also
========
#TODO