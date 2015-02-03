========
reversed
========

Description
===========
Returns a reverse iterator over a sequence.

Syntax
======
**reversed** *(sequence)*

*sequence*
	Required. Any iterable sequence.

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
sequence must be an object which has a __reversed__() method or supports the sequence protocol (the __len__() method and the __getitem__() method with integer arguments starting at 0).

Example 1
=========
>>> r = reversed([1, 2])
>>> r.next()
2
>>> r.next()
1
>>> r.next()
Traceback (most recent call last):
  File "<interactive input>", line 1, in <module>
StopIteration

Example 2
=========
>>> for r in reversed((1, 2)):
...     print r
...
2
1

See Also
========
#TODO