====
bool
====

Description
===========
Returns an expression converted into a Boolean.

Syntax
======
**bool** *(expression)*

*expression*
	Required. If expression is False or omitted, this returns False; otherwise it returns True.

Return Value
============
**bool**

Time Complexity
============
#TODO

Remarks
=======
**bool** is also a class, which is a subclass of **int**. Class **bool** cannot be subclassed further. Its only instances are **False** and **True**.

The following values are interpreted as false:

* False

* None

* numeric zero of all types

* empty strings and containers (including strings, tuples, lists, dictionaries, sets and frozensets)

All other values are interpreted as true. (See the __nonzero__() special method for a way to change this.)

Example
=======
>>> bool(1)
True
>>> bool(0)
False
>>> bool("False")
True
>>> bool([0, 0])
True
>>> bool([])
False
>>> bool(2+2)
True

See Also
========
#TODO

