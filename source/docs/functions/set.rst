===
set
===

Description
===========
Returns a set type initialized from iterable.

Syntax
======
**set** *([iterable])*

*iterable*
	Required. All of the elements in iterable should be immutable.

Return Value
============
**set**

Time Complexity
============
#TODO

Remarks
=======
Set is an unordered, mutable collection of unique elements. See frozenset() for the immutable version.

Example
=======
>>> set()
set([])
>>> set([1, 2, 2])
set([1, 2])
>>> set({'a': 1, 'b': 2})
set(['a', 'b'])
>>> set('foo')
set(['f', 'o'])

See Also
========
#TODO