===
min
===

Description
===========
Returns the smallest item from a collection.

Syntax
======
**min** *(collection[, key])*

collection*
	Required. A comma-separated list of objects or an iterable sequence.
key*
	Optional. Specifies a one-argument ordering function; must be in keyword form.

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
When comparing sequences lexical comparison is used.

Example 1
=========
>>> min(1, 2, 3)
1
>>> min('A', 'a', 'b')
'A'
>>> min([1, 2], [2, 1], [3, 1])
[1, 2]
>>> min(str([1, 2]), str([2, 1]), str([3, 1]))
'[1, 2]'

Example 2
=========
>>> min('apple', 'Pear', key=lambda x: x.upper())
'apple'
>>> min('apple', 'Pear')
'Pear'

See Also
========
#TODO
