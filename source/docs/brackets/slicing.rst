==============
[] (slicing)
==============

Description
===========
Gives access to a specified range of sequence's elements.

Syntax
======
**sequence** *[start:stop[:step]]*

*start*
    Optional. Starting index of the slice. Defaults to 0.
*stop*
    Optional. The last index of the slice or the number of items to get. Defaults to *len(sequence)*.
*step*
    Optional. Extended slice syntax. Step value of the slice. Defaults to 1.

Return Value
============
The same as selected.

Time Complexity
===============
O(k) for slice retrieval

O(n) for deletion

O(n+k) for slice assignment

Remarks
=======
Consider the following ASCII graph showing the contents of the "ABCD" string:

>>> +---+---+---+---+
>>> |-4 |-3 |-2 |-1 |  <= negative indexes
>>> +---+---+---+---+
>>> | A | B | C | D |  <= sequence elements
>>> +---+---+---+---+
>>> | 0 | 1 | 2 | 3 |  <= positive indexes
>>> +---+---+---+---+
>>> |<- 0:3:1 ->|      <= extent of the slice: "ABCD"[0:3:1]


Consider the following example:

Example 1
=========
>>> "ABCD"[0:2]
'AB'

It can be read as: get every single one item between indexes 0 and 2 (exclusive).

The next example shows usage of the *step* argument:

Example 2
=========
>>> "ABCD"[0:4:2]
'AC'

That can be interpreted as: get every second element between indexes 0 and 4.

Usage of start, stop and step operators is optional:

Example 3
=========
>>> "ABCD"[1:]
'BCD'
>>> "ABCD"[:3]
'ABC'
>>> "ABCD"[1:3]
'BC'
>>> "ABCD"[1:3:]
'BC'
>>> "ABCD"[::2]
'AC'
>>> "ABCD"[::]
'ABCD'
>>> "ABCD"[:]
'ABCD'

Negative step argument can be used to reverse the sequence:

Example 4
=========
>>> "ABCD"[::-1]
'DCBA'
>>> [0, 1, 2, 3][::-1]
[3, 2, 1, 0]

Example 5
=========
>>> # slices can be used to replace multiple items
>>> l = [0, 1, 2, 3]
>>> l[:2] = ("AB", "CD")
>>> l
['AB', 'CD', 2, 3]

Example 6
=========
>>> l = [0, 1, 2, 3]
>>> l[1:2] = (7, 8, 9, 10)
>>> l
[0, 7, 8, 9, 10, 2, 3]

Example 7
=========
>>> # when using extended slice syntax both chunks must match
>>> l = [0, 1, 2, 3]
>>> l[::2] = "ABCD"
Traceback (most recent call last):
  File "<interactive input>", line 1, in <module>
ValueError: attempt to assign sequence of size 4 to extended slice of size 2

Example 8
=========
>>> # deleting items
>>> l = [0, 1, 2, 3]
>>> del l[::2]
>>> l
[1, 3]

See Also
========
#TODO
