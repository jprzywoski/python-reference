====
list
====

Description
===========
Converts an object into a list.

Syntax
======
**list** *([iterable])*

*iterable*
	Optional. Any iterable.

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
list() returns a list whose items are the same and in the same order as iterable‘s items. iterable may be either a sequence, a container that supports iteration, or an iterator object. If iterable is already a list, a copy is made and returned, similar to iterable[:]. For instance, list('abc') returns ['a', 'b', 'c'] and list( (1, 2, 3) ) returns [1, 2, 3]. If no argument is given, returns a new empty list, [].

Example
=======
>>> list('foo')
['f', 'o', 'o']
>>> list((1, 2))
[1, 2]
>>> list({1, 2})
[1, 2]
>>> list({'a': 1, 'b': 2})
['a', 'b']
>>> list([1, 2])
[1, 2]
>>> list()
[]
>>> list(iter([1, 2]))
[1, 2]

See Also
========
#TODO