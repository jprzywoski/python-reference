======
sorted
======

Description
===========
Returns a sorted list from the iterable.

Syntax
======
**sorted** *(iterable[, cmp[, key[, reverse]]])*

*iterable*
	Required.
*cmp*
	Optional. A custom comparison function of two arguments (iterable elements) which should return a negative, zero or positive number depending on whether the first argument is considered smaller than, equal to, or larger than the second argument. The default value is None.
*key*
	Optional. A function of one argument that is used to extract a comparison key from each list element. The default value is None (compare the elements directly).
*reverse*
	Optional. Boolean value. If set to True, then the list elements are sorted as if each comparison were reversed.

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
In general, the key and reverse conversion processes are much faster than specifying an equivalent cmp function. This is because cmp is called multiple times for each list element while key and reverse touch each element only once. Use functools.cmp_to_key() to convert an old-style cmp function to a key function.
For sorting examples and a brief sorting tutorial, see Sorting HowTo.

Example 1
=========
>>> sorted('foobar')
['a', 'b', 'f', 'o', 'o', 'r']
>>> sorted((3, 1, 2))
[1, 2, 3]
>>> sorted([3, 1, 2])
[1, 2, 3]
>>> sorted({3, 1, 2})
[1, 2, 3]
>>> sorted({'a': 1, 'c': 3, 'b': 2})
['a', 'b', 'c']

Example 2
=========
>>> sorted({'a': 1, 'c': 3, 'b': 2}, reverse=True)
['c', 'b', 'a']
>>> sorted({1, 3, 2}, reverse=True)
[3, 2, 1]
>>> sorted((1, 3, 2), reverse=True)
[3, 2, 1]
>>> sorted('foobar', reverse=True)
['r', 'o', 'o', 'f', 'b', 'a']

Example 3
=========
>>> sorted(['pear', 'apple', 'pineapple'])
['apple', 'pear', 'pineapple']
>>> sorted(['pear', 'apple', 'pineapple'], cmp=lambda x, y: cmp(len(x), len(y)))
['pear', 'apple', 'pineapple']

Example 4
=========
>>> sorted(['A', 'b', 'C'])
['A', 'C', 'b']
>>> sorted(['A', 'b', 'C'], key=lambda x: x.lower())
['A', 'b', 'C']
>>> sorted(((1, ), (1, 2, 3), (1, 2)))
[(1,), (1, 2), (1, 2, 3)]
>>> sorted(((9, ), (1, 2, 3), (1, 2)), key=lambda x: sum(x))
[(1, 2), (1, 2, 3), (9,)]

See Also
========
#TODO