==
is
==

Description
===========
Returns a Boolean stating whether two variables are referencing the same object.

Syntax
======
A is [not] B

Remarks
=======
Equivalent to id(A) == id(B). Note that two different objects can have the same value.

Example 1
=========
>>> a = 'foo'
>>> b = 'foo'
>>> a is b
True

Example 2
=========
>>> a = 'Arbeitsunfaehigkeitbescheinigung-' # certificate of inability to work in German
>>> b = 'Arbeitsunfaehigkeitbescheinigung-'
>>> a is b
False
>>> a == b
True
>>> id(a)
14418904
>>> id(b)
14418288