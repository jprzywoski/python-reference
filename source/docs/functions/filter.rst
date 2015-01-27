filter
======

Description
-----------
Returns a sequence from those elements of iterable for which function returns true.

Syntax
------
**filter** (*function*, *iterable*)

*function*
    Required. A function. If set to None returns only elements that are True.
    
*iterable*
    Required. Any iterable sequence.
    
Return Value
------------
same as returned by *function*

Time Complexity
---------------
#TODO

Note
----
Note that filter(function, iterable) is equivalent to [item for item in iterable if function(item)] if function is not None and [item for item in iterable if item] if function is None.
See itertools.ifilter() and itertools.ifilterfalse() for iterator versions of this function, including a variation that filters for elements where the function returns false.

Example 1
---------
>>> def f(x):
...     if x > 0:
...         return x
>>> filter(f, [-1, 0, 1])
[1]

Example 2
---------
>>> filter(None, (0, 1, True))
(1, True)

See Also
--------
`map()`_, `reduce()`_, `comprehensions and generator expressions`_.

.. _map(): ../functions/map.html
.. _reduce(): ../functions/reduce.html
