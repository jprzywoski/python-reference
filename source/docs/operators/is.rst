====
is
====

Description
===========
Returns a Boolean stating whether two objects are the same.

Syntax
======
A is [not] B

*A*
    Any object.
*B*
    Any object.

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
Equivalent to id(A) == id(B). Note that two different objects can have the same value. 

Example 1
=========
>>> a = 'ABCD'
>>> b = 'ABCD'
>>> a is b
True

Example 2
=========
>>> a = 'Arbeitsunfähigkeitbescheinigung-' # certificate of inability to work in German
>>> b = 'Arbeitsunfähigkeitbescheinigung-'
>>> a is b
False
>>> a == b
True
>>> id(a)
14418904
>>> id(b)
14418288

See also
========
intern() and id() functions, equals operator

