===
any
===

Description
===========
Returns a Boolean value that indicates whether the collection contains any values that evaluate to True.

Syntax
======
**any** *(iterable)*

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
If the iterable is empty, returns False.

Example
=======
>>> any([True, True])
True
>>> any([True, False])
True
>>> any([False, False])
False
>>> any('False')
True
>>> any([])
False

See Also
========
#TODO