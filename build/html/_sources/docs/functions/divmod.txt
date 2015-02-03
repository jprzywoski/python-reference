======
divmod
======

Description
===========
Returns quotient and remainder after a division of two numbers.

Syntax
======
**divmod** *(number1, number2)*

*number1, number2*
	Required. Any numeric expression.

Return Value
============
**tuple**

Time Complexity
============
#TODO

Note
====
Using divmod() with complex numbers is deprecated.

Remarks
=======
With mixed operand types, the rules for binary arithmetic operators apply. For plain and long integers, the result is the same as (a // b, a % b). For floating point numbers the result is (q, a % b), where q is usually math.floor(a / b) but may be 1 less than that. In any case q * b + a % b is very close to a, if a % b is non-zero it has the same sign as b, and 0 <= abs(a % b) < abs(b).

Example
=======
>>> divmod(10, 3)
(3, 1)
>>> divmod(10.5, 3)
(3.0, 1.5)
>>> divmod(10.5, 3.1)
(3.0, 1.1999999999999997)
>>> divmod(10.5, 3.5)
(3.0, 0.0)

See Also
========
#TODO