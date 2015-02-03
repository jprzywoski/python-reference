=====
slice
=====

Description
===========
Returns a slice object.

Syntax
======
**slice** *(stop)*
**slice** *(start, stop[, step])*

*start*
	Required if stop is used. Starting index.
*stop*
	Required. Last item plus one returned by the slice
*step*
	Optional. Value of the step.

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
Slice objects have read-only data attributes start, stop and step which merely return the argument values (or their default). They have no other explicit functionality; however they are used by Numerical Python and other third party extensions. Slice objects are also generated when extended indexing syntax is used. For example: a[start:stop:step] or a[start:stop, i]. See itertools.islice() for an alternate version that returns an iterator.

Example
=======
>>> slice(0, 5, 2)
slice(0, 5, 2)

See Also
========
#TODO