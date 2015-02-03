===
sum
===

Description
===========
Returns a total of the items contained in the iterable object.

Syntax
======
**sum** *(iterable[, start])*

*iterable*
	Required. An iterable object.
*start*
	Optional. An integer specifying the start value.

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
For some use cases, there are good alternatives to sum(). The preferred, fast way to concatenate a sequence of strings is by calling “”.join(sequence). To add floating point values with extended precision, see math.fsum(). To concatenate a series of iterables, consider using itertools.chain().

Example 1
=========
>>> sum([1, 2, 3])
6 # 1+2+3
>>> sum((1, 2, 3))
6
>>> sum({1, 2, 3})
6
>>> sum({1: 'a', 2: 'b', 3: 'c'})
6

Example 2
=========
>>> sum([1, 2, 3], 10)
16 # 10+1+2+3
>>> sum((1, 2, 3), 10)
16
>>> sum({1, 2, 3}, 10)
16
>>> sum({1: 'a', 2: 'b', 3: 'c'}, 10)
16

Example 3
=========
>>> sum([0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1])
0.9999999999999999
>>> import math
>>> math.fsum([0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1])
1.0

See Also
========
#TODO
