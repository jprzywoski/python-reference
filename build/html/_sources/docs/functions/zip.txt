===
zip
===

Description
===========
Returns a list of tuples, where the i-th tuple contains the i-th element from each of the argument sequences or iterables.

Syntax
======
**zip** *([iterable, ...])*

*iterable*
	Optional. An iterable object.

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
The returned list is truncated in length to the length of the shortest argument sequence. When there are multiple arguments which are all of the same length, zip() is similar to map() with an initial argument of None. With a single sequence argument, it returns a list of 1-tuples. With no arguments, it returns an empty list.

The left-to-right evaluation order of the iterables is guaranteed. This makes possible an idiom for clustering a data series into n-length groups using zip(*[iter(s)]*n).

Example 1
=========
>>> zip()
[]
>>> zip('foo', 'bar')
[('f', 'b'), ('o', 'a'), ('o', 'r')]
>>> zip((1, 1), (2, 4))
[(1, 2), (1, 4)]
>>> zip((1, 2), (3, 4))
[(1, 3), (2, 4)]
>>> zip([1, 2], [3, 4])
[(1, 3), (2, 4)]

Example 2
=========
>>> #zip() in conjunction with the * operator can be used to unzip a list:
>>> x = [1, 2, 3]
>>> y = [4, 5, 6]
>>> zipped = zip(x, y)
>>> zipped
[(1, 4), (2, 5), (3, 6)]
>>> x2, y2 = zip(*zipped)
>>> x == list(x2) and y == list(y2)
True

Example 3
=========
>>> zip((1, 2, 3), (4, 5))
[(1, 4), (2, 5)]
>>> zip((1, 2), (3, 4), (5, 6))
[(1, 3, 5), (2, 4, 6)]
