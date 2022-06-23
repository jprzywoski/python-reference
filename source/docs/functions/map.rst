map
===

Description
-----------
Applies function to every item of an iterable and returns an iterable of the results.

Syntax
------

**map** *(function, iterable [, ...])*

*function*
    Required. A function that is used to create a new list.
*iterable*
    Required. An iterable object or multiple comma-seperated iterable objects.
    
Return Value
------------
map object

Time Complexity
------------
#TODO

Remarks
-------
If additional *iterable* arguments are passed, function must take that many arguments and is applied to the items from all iterables in parallel. If one *iterable* is shorter than another it is assumed to be extended with **None** items. If function is None, the identity function is assumed; if there are multiple arguments, map() returns a list consisting of tuples containing the corresponding items from all iterables (a kind of transpose operation). The *iterable* arguments may be a sequence or any iterable object; the result is always an iterable, a map object to be precise.

The function will not be applied to the parameter iterable until the result iterable is called (transformed into list, popped first item, etc.). This can be done by calling e.g. next() or list() on the result (see examples).

Example 1
---------
>>> map(lambda x: x+x, (1, 2, 3))
<map object at 0x0000014BC76494C0>
>>> list(map(lambda x, y: x/y, (1, 4, 9), (1, 2, 3)))
[1, 2, 3]
>>> list(map(lambda x, y, z: x+y+z, (1, 2, 3), (1, 4, 9), (1, 16, 27)))
[3, 22, 39]

Example 2
---------
>>> list(map(None, [True, False]))
[True, False]
>>> list(map(None, ['a', 'b'], [1, 2]))
[('a', 1), ('b', 2)]
>>> list(map(None, ['a', 'b'], [1, 2, 3]))
[('a', 1), ('b', 2), (None, 3)]

See Also
--------
`reduce()`_, `filter()`_ and `Comprehensions and Generator Expression`_.

.. _reduce(): reduce.html
.. _filter(): filter.html
.. _Comprehensions and Generator Expression: ../comprehensions/index.html

