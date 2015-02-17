===
and
===

Description
===========
Returns the first operand that evaluates to *False* or the last one if all are *True*.

Syntax
======
**A and B**

*A*
    Any valid object.
*B*
    Any valid object.
    
Return Value
============
The same as passed to the expression.

Time Complexity
============
#TODO

Remarks
=======
In the context of Boolean operations, and also when expressions are used by control flow statements, the following values are interpreted as false: False, None, numeric zero of all types, and empty strings and containers (including strings, tuples, lists, dictionaries, sets and frozensets). All other values are interpreted as true. (See the __nonzero__() special method for a way to change this.)

The expression:

>>> x and y

first evaluates x; if x is false, its value is returned; otherwise, y is evaluated and the resulting value is returned.

Example 1
====
>>> 0 and '' and False
0
>>> 1 and '' and False
''
>>> 1 and 'A' and False
False
>>> 1 and 2 and 3
3

Example 2
====
>>> b = '' and 'ABCD'
>>> b
''
>>> b = 0 and 1
>>> b
0

See Also
========
#TODO