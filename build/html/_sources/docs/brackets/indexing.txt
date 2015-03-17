========================
[] (index operator)
========================

Description
===========
Gives access to a sequence's element.

Syntax
======
**sequence** *[index]*

*index*
    Index of the item you want to access. Must be an integer.

Return Value
============
The same as selected.

Time Complexity
===============
O(1)

Discussion
==========
The built-in fundamental sequence types are:

* strings - str and unicode
* arrays - list and tuple

Since all sequences are ordered and indexed arrays of objects, each object stored in a sequence has it's associated index number - positive one, zero indexed and starting from left, and the negative one starting at -1 from the right.

Consider the following ASCII graph showing the contents of the "ABCD" string:

>>> +---+---+---+---+
>>> |-4 |-3 |-2 |-1 |  <= negative indexes
>>> +---+---+---+---+
>>> | A | B | C | D |  <= sequence elements
>>> +---+---+---+---+
>>> | 0 | 1 | 2 | 3 |  <= positive indexes
>>> +---+---+---+---+

Remarks
=======
The number of items in a sequence cam be retrieved by using `len()`_ function:

>>> len("ABCD")
4
>>> len([0, 1, 2])
3

Trying to access an element out of range throws an IndexError.

Example 1
=========
>>> # this example show how to retrieve elements of a sequence
>>> "ABCD"[0]
'A'
>>> [0, 1, 2][1]
1
>>> ("ABC", "DEF", "GHI")[1]
'DEF'

Example 2
=========
>>> # index lookups can be chained to access nested containers
>>> ([0, 1], [2, 3])[1][1]
3

Example 3
=========
>>> # using negative indexes to get the last element
>>> (0, 1, 2)[-1]
2
>>> "ABCD"[-1]
'D'

Example 4
=========
>>> # since lists are mutable indexes can be used for item assignment or deletion
>>> l = [0, 1, 2, 3]
>>> l[0] = "ABCD"
>>> l
['ABCD', 1, 2, 3]

Example 5
=========
>>> l = [0, 1, 2, 3]
>>> del l[2]
>>> l
[0, 1, 3]

See Also
========
#TODO

