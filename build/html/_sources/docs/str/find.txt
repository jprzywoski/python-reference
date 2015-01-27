====
find
====

Description
----------
Returns the index of the first occurrence of the string searched for.

Syntax
------
**str**. *find(sub[, start[, end]])*

*sub*
    Required. The string searched for.
*start*
    Optional. Search start position.
*end*
    Optional. Search end position.

Return Value
------------
**int**

Time Complexity
---------------
#TODO

Remarks
-------
Returns -1 if *sub* is not found.

The find() method should be used only if you need to know the position of *sub*. To check if *sub* is a substring or not, use the **in** operator:

>>> 'Py' in 'Python'
True

Example
-------
>>> "ABAB".find("B")
1
>>> "ABAB".find("B", 2, 4)
3
>>> "ABAB".find("B", 2)
3

See Also
--------
`rfind()`_

`index()`_

`rindex()`_

.. _rfind(): ../bd_strings/rfind.html
.. _index(): ../bd_strings/strindex.html
.. _rindex(): ../bd_strings/rinddex.html
