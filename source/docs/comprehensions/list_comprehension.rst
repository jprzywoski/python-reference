=====================
[] list comprehension
=====================

Description
===========
Returns a list based on existing iterables.

Syntax
======
**[expression(variable) for variable in input_set [predicate][, …]]**

*expression*
	Optional. An output expression producing members of the new set from members of the input set that satisfy the predicate expression.
*variable*
	Required. Variable representing members of an input set.
*input_set*
	Required. Represents the input set.
*predicate*
	Optional. Expression acting as a filter on members of the input set.
*[, …]]*
	Optional. Another nested comprehension.

Return Value
============
**list**

Time Complexity
===============
#TODO

Remarks
=======
A list comprehension follows the form of the mathematical set-builder notation (set comprehension) as distinct from the use of `map()`_ and `filter()`_ functions.

Consider the following example:

>>> l = [2 * n for n in (0, 1, 2) if n > 0]
>>> l
[2, 4]

This can be read as: 

*l* is the list of all numbers *2 times n* where *n* is an item in the *(0, 1, 2)* tuple, for which tuple element is greater than zero.

Example 1
=========
>>> [n for n in [1, 2, 3]]
[1, 2, 3]
>>> [n * 2 for n in [1, 2, 3]]
[2, 4, 6]
>>> [n**2 for n in range(10)]
[0, 1, 4, 9, 16, 25, 36, 49, 64, 81]

Example 2
=========
>>> [n for n in [1, 2, 3] if n % 2]  # odd numbers only
[1, 3]

Example 3
=========
>>> [[m, n] for n in [0, 2] for m in [1, 2]]
[[1, 0], [2, 0], [1, 2], [2, 2]]
>>> [[m, n] for n in [i for i in [0, 1]] for m in [1, 2]]
[[1, 0], [2, 0], [1, 1], [2, 1]]
       
See Also
========
#TODO

.. _map(): ../functions/map.html
.. _filter(): ../functions/filter.html

