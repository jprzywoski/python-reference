======
xrange
======

Description
===========
Returns an xrange object.

Syntax
======
**xrange** *(stop)*
**xrange** *(start, stop[, step])*

*start*
	Required when full syntax is used. An integer specifying start value for the range.
*stop*
	Required. The boundary value for the range.
*step*
	Optional. Step value.

Return Value
============
#TODO

Time Complexity
============
#TODO

Note
====
CPython implementation detail: xrange() is intended to be simple and fast. Implementations may impose restrictions to achieve this. The C implementation of Python restricts all arguments to native C longs (“short” Python integers), and also requires that the number of elements fit in a native C long. If a larger range is needed, an alternate version can be crafted using the itertools module: islice(count(start, step), (stop-start+step-1+2*(step<0))//step).

Remarks
=======
This function is very similar to range(), but returns an xrange object instead of a list. This is an opaque sequence type which yields the same values as the corresponding list, without actually storing them all simultaneously. The advantage of xrange() over range() is minimal (since xrange() still has to create the values when asked for them) except when a very large range is used on a memory-starved machine or when all of the range’s elements are never used (such as when the loop is usually terminated with break). For more information on xrange objects, see XRange Type and Sequence Types — str, unicode, list, tuple, bytearray, buffer, xrange.

Example
=======
>>> for i in xrange(10):
...     print i
...
0
1
2
3
4
5
6
7
8
9

See Also
========
#TODO