==
or
==

Description
===========
Returns the first operand that evaluates to *True* or the last one if all are *False*.

Syntax
======
**A or B**

*A*
    Any valid object.
*B*
    Any valid object.

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
In the context of Boolean operations, and also when expressions are used by control flow statements, the following values are interpreted as false: False, None, numeric zero of all types, and empty strings and containers (including strings, tuples, lists, dictionaries, sets and frozensets). All other values are interpreted as true. (See the __nonzero__() special method for a way to change this.)

The expression:

>>> x or y

first evaluates x; if x is true, its value is returned; otherwise, y is evaluated and the resulting value is returned.

Example 1
====
>>> 0 or '' or False
False
>>> 1 or '' or False
1
>>> 1 or 'A' or False
1
>>> 1 or 2 or 3
1

Example 2
====
>>> b = '' or 'ABCD'
>>> b
'ABCD'
>>> b = 0 or 1
>>> b
1

See Also
========
#TODO