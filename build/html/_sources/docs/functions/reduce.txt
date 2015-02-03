reduce
======

Description
-----------
Applies function of two arguments cumulatively to the items of iterable, from left to right, so as to reduce the iterable to a single value.

Syntax
------

**reduce** *(function, iterable [, initializer])*

*function*
    Required. A function of two arguments.
*iterable*
    Required. An iterable sequence.
*initializer*
    Optional. Value placed before the iterable; default value if iterable is empty.
    
Return Value
------------
same as returned by *function*

Time Complexity
---------------
#TODO

Example 1
---------
>>> reduce(lambda x, y: x+y, [1, 2, 3, 4]) # the left argument, x, is the accumulated value and the right argument, y, is the update value from the iterable.
10 # ((1+2)+3)+4) 
>>> reduce(lambda x, y: x-y, [125, 25, 5, 1])
94 # ((125-25)-5)-1)
>>> reduce(lambda x, y: x*y, [2, 2, 2, 2])
16 # ((2*2)*2)*2)
>>> reduce(lambda x, y: x/y, [125, 25, 5, 1])
1 # ((125/25)/5)/1)
>>> reduce(lambda x, y: x*y, [1])
1

Example 2
---------
>>> reduce(lambda x, y: x+y, [], 1)
1
>>> reduce(lambda x, y: x+y, [], 0)
0
>>> reduce(lambda x, y: x*y, [1, 2, 3], 0)
0 # because ((0*1)*2)*3)

See Also
--------
`map()`_, `filter()`_ and `Comprehensions and Generator Expression`_.

.. _map(): map.html
.. _filter(): filter.html
.. _Comprehensions and Generator Expression: ../comprehensions/index.html

