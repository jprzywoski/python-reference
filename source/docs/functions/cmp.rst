===
cmp
===

Description
===========
Compares two objects and returns an integer according to the outcome.

Syntax
======
**cmp** *(object1, object2)*

*object1, object2*
	Required. If objects are of a sequence type cmp performs lexical comparison. The return value is -1 if object1 < object2, 0 if object1 == object2 and 1 if object1 > object2.

Return Value
============
#TODO

Time Complexity
============
#TODO

Example
=======
>>> cmp(1, 2)
-1
>>> cmp(0, 1)
-1
>>> cmp(1, 1)
0
>>> cmp(1, 2)
-1
>>> cmp('foo', 'bar')
1
>>> cmp([1, 2], [2, 1])
-1

See Also
========
#TODO