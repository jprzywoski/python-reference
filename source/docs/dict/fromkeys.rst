========
fromkeys
========

Description
===========
Returns a new dictionary with keys from a supplied iterable and values all set to specified value.

Syntax
======
**dict**. *fromkeys(iterable[, value])*

*iterable*
    Required. Any iterable.
*value*
    Optional. Default value for the keys. Default value is **None**.

Return Value
============
**dict**

Time Complexity
===============
#TODO

Example 1
=========
>>> l = [1, 2, 3]
>>> d = {}
>>> d.fromkeys(l)
{1: None, 2: None, 3: None}

Example 2
=========
>>> d = {}.fromkeys([1, 2, 3], "NULL")
>>> d
{1: 'NULL', 2: 'NULL', 3: 'NULL'}

See Also
========
#TODO
