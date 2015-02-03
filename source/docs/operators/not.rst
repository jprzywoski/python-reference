===
not
===

Description
===========
Reverts the logical state of a condition.

Syntax
======
not A

Example
======= 1
>>> not True
False
>>> not False
True

Example
======= 2
>>> True and not False
True
>>> True and not True
False
>>> True or not True
True
>>> True or not False
True