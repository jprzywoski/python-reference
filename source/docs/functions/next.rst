====
next
====

Description
===========
Retrieves the next item from the iterator by calling its next() method.

Syntax
======
**next** *(iterator[, default])*

*iterator*
	Required. An iterator object.
*default*
	Optional. This is the value that is returned after retrieving the last item instead of StopIteration error.

Return Value
============
#TODO

Time Complexity
============
#TODO

Example 1
=========
>>> i = iter([1, 2])
>>> next(i)
1
>>> next(i)
2
>>> next(i)
Traceback (most recent call last):
  File "<interactive input>", line 1, in <module>
StopIteration

Example 2
=========
>>> i = iter([1, 2])
>>> next(i, 'No more items in the list.')
1
>>> next(i, 'No more items in the list.')
2
>>> next(i, 'No more items in the list.')
'No more items in the list.'

See Also
========
#TODO
