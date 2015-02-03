=========
frozenset
=========

Description
===========
Returns a frozenset object.

Syntax
======
**frozenset** *(iterable)*

*iterable*
	Optional. An iterable sequence from which the frozenset is created.

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
Frozenset is an immutable version of set object.

Example
=======
>>> frozenset([1, 1, 2])
frozenset([1, 2])
>>> frozenset('foobar')
frozenset(['a', 'b', 'f', 'o', 'r'])
>>> frozenset((1, 2, 3))
frozenset([1, 2, 3])
>>> frozenset({'a': 1, 'b': 2})
frozenset(['a', 'b'])
>>> frozenset({1, 2})
frozenset([1, 2])
>>> fs = frozenset([1, 2, 3])
>>> fs[1] = 10
Traceback (most recent call last):
  File "<interactive input>", line 1, in <module>
TypeError: 'frozenset' object does not support item assignment

See Also
========
#TODO