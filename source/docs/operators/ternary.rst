=======================================
... if ... else ... Ternary Conditional
=======================================

Description
===========
Returns either value depending on the result of a Boolean expression.

Syntax
======
VARIABLE if EXPRESSION else VARIABLE

Remarks
=======
Conditional expressions or ternary operator have the lowest priority of all Python operations. The expression first evaluates the condition, C (not x); if C is true, x is evaluated and its value is returned; otherwise, y is evaluated and its value is returned.

Example
======= 1
>>> 1 if True else 0
1
>>> 1 if False else 0
0

Example
======= 2
>>> 1 if 2 + 2 == 4 else 0
1
>>> 1 if 2 + 2 != 4 else 0
0