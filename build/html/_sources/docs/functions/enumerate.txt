=========
enumerate
=========

Description
===========
Returns an enumerate object.

Syntax
======
**enumerate** *(sequence, start=0)*

*sequence*
	Required. Must be a sequence, an iterator, or some other object which supports iteration.
*start*
	Optional. Index at which enumeration starts.

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
The next() method of the iterator returned by enumerate() returns a tuple containing a count (from start which defaults to 0) and the values obtained from iterating over sequence.

Example 1
=========
>>> for i in enumerate((1, 2, 3)):
...     print i
...
(0, 1)
(1, 2)
(2, 3)

Example 2
=========
>>> e = enumerate([1, 2])
>>> e.next()
(0, 1)
>>> e.next()
(1, 2)
>>> e.next()
Traceback (most recent call last):
  File "<interactive input>", line 1, in <module>
StopIteration

Example 3
=========
>>> e = enumerate([1, 2, 3], 1)
>>> e = enumerate([1, 2, 3], start=1)
>>> e.next()
(1, 1)
>>> e.next()
(2, 2)
>>> e.next()
(3, 3)
>>> e.next()

See Also
========
#TODO