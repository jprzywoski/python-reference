===
pow
===

Description
===========
Returns a number raised to a power; or optionally a modulus of the number raised to a power and another number.

Syntax
======
**pow** *(base, power[, number])*

*base*
	Required. The number to be raised to a power.
*power*
	Required. The power/index.
*number*
	Optional. The number used for division of the result of the base**power expression.

Return Value
============
**int** or **float**

Time Complexity
============
#TODO

Remarks
=======
The three argument form is computed more efficiently than pow(base, power) % number. The two-argument form pow(base, power) is equivalent to using the power operator: base**power.

The arguments must have numeric types. With mixed operand types, the coercion rules for binary arithmetic operators apply. For int and long int operands, the result has the same type as the operands (after coercion) unless the second argument is negative; in that case, all arguments are converted to float and a float result is delivered. For example, 10**2 returns 100, but 10**-2 returns 0.01. If the second argument is negative, the third argument must be omitted. If number is present, base and power must be of integer types, and power must be non-negative.

Example 1
=========
>>> pow(2, 2)
4
>>> pow(2, -2)
0.25

Example 2
=========
>>> pow(2.0, -2.0)
0.25
>>> pow(2.0, 1.0/2.0)
1.4142135623730951

Example 3
=========
>>> pow(10, 2, 9)
1 #equivalent to remainder of (10**10)/9

See Also
========
#TODO