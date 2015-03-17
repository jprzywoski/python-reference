====
in
====

Description
===========
Returns a Boolean stating whether the object is in the container.

Syntax
======
A [not] in B

*A*
    Any valid object.
*B*
    Any valid object.

Return Value
============
#TODO

Time Complexity
============
O(1) for dict
O(1) to O(n) for sets
O(n) for sequences (str, list, tuple)


Remarks
=======
When used with dictionaries checks the keys instead of values.
    
Example
=======
>>> 'A' in 'ABCD'
True
>>> 0 in [0, 1, 2]
True
>>> 0 not in {'a': 0, 'b': 1}
True

See also
========
#TODO