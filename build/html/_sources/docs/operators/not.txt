===
not
===

Description
===========
Returns a boolean that is the reverse of the logical state of an expression.

Syntax
======
**not A**

*A*
    Any valid object.

Return Value
============
*bool*

Time Complexity
============
#TODO

Remarks
=======
Note that *not* does not return the evaluated argument but a Boolean instead.

Example 1
========
>>> not True
False
>>> not False
True

Example 2
=======
>>> True and not False
True
>>> True and not True
False
>>> True or not True
True
>>> True or not False
True

See Also
========
#TODO