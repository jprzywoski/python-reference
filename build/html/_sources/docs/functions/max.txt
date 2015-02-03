===
max
===

Description
===========
Returns the largest item in an iterable or the largest of two or more arguments.

Syntax
======
**max** *(collection[, key])*

*colllection*
	Required. A comma-separated list of objects or an iterable sequence.
*key*
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

Example
=======
>>> max(1, 2, 3)
3
>>> max('A', 'a', 'b')
'b'
>>> max([1, 2], [2, 1], [3, 1])
[3, 1]
>>> max(str([1, 2]), str([2, 1]), str([3, 1]))
'[3, 1]'

Example 2
=========
>>> max('apple', 'Pear', key=lambda x: x.upper())
'Pear'
>>> max('apple', 'Pear')
'apple'

See Also
========
#TODO
