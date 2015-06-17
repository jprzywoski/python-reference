====
sort
====

Description
===========
Sorts the list in place.

Syntax
======
**list**. *sort([cmp[, key[, reverse]]])*

*cmp*
    Optional. Specifies a custom comparison function of two arguments (list items) which should return a negative, zero or positive number depending on whether the first argument is considered smaller than, equal to, or larger than the second argument: The default value is **None**.
*key*
    Optional. Specifies a function of one argument that is used to extract a comparison key from each list element. The default value is **None**.
*reverse*
    Optional. A boolean value. If set to **True**, then the list elements are sorted as if each comparison were reversed.

Return Value
============
**None**

Time Complexity
===============
O(n log n)

Remarks
=======
In general, the *key* and *reverse* conversion processes are much faster than specifying an equivalent *cmp* function. This is because *cmp* is called multiple times for each list element while *key* and *reverse* touch each element only once.

Example 1
=========
>>> l = [1, 3, 2]
>>> l.sort()
>>> l
[1, 2, 3]

Example 2
=========
>>> # this example shows how to use cmp argument
>>> l = ['a', 'B', 'A', 'c']
>>> l.sort()
>>> l
['A', 'B', 'a', 'c']
>>> l = ['a', 'B', 'A', 'c']
>>> l.sort(lambda x, y: cmp(x.lower(), y.lower()))
>>> l
['a', 'A', 'B', 'c']

Example 3
=========
>>> l = ['a', 'B', 'c']
>>> l.sort()
>>> l
['B', 'a', 'c']
>>> l.sort(key=lambda x: x.lower())
>>> l
['a', 'B', 'c']

Example 4
=========
>>> l = [1, 3, 2]
>>> l.sort()
>>> l
[1, 2, 3]
>>> l.sort(reverse=True)
>>> l
[3, 2, 1]

See Also
========
`sorted()`_ function

.. _sorted: ../functions/sorted.html
