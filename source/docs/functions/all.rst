===
all
===

Description
===========
Returns a Boolean value that indicates whether the collection contains only values that evaluate to True.

Syntax
======
**all** *(iterable)*

*iterable*
	Required. Any iterable type.

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
If the iterable is empty, all() returns True.

Example 1
=========
>>> all([])
True
>>> all([True, False])
False
>>> all([True, True])
True

Example 2
=========
>>> all('True')
True
>>> all('False') # note that non-empty strings are always True
True
>>> all([0, 1])
False
>>> all([1, 1])
True
>>> all((1, 1))
True
>>> all((1, 0))
False
>>> all({0: 'zero', 1: 'one'})
False
>>> all({1: 'one', 2: 'two'})
True
>>> all({0, 1})
False
>>> all({1, 1})
True

See Also
========
#TODO