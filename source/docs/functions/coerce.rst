======
coerce
======

Description
===========
Returns a tuple consisting of the two numeric arguments converted to a common type.

Syntax
======
**coerce** *(number1, number2)*

*number1, number2*
	Required.  Any numeric type.

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
Coercion is the implicit conversion of an instance of one type to another during an operation which involves two arguments of the same type. For example, in 3+4.5, each argument is of a different type (one int, one float), and both must be converted to the same type before they can be added or it will raise a TypeError. Coercion between two operands can be performed with the coerce built-in function; thus, 3+4.5 is equivalent to calling operator.add(*coerce(3, 4.5)) and results in operator.add(3.0, 4.5). Without coercion, all arguments of even compatible types would have to be normalized to the same value by the programmer, e.g., float(3)+4.5 rather than just 3+4.5.
If coercion is not possible, coerce raises TypeError. Use of the coerce function is in not really necessary since Python’s interpreter automatically normalizes values in arithmetic expressions.

Example 1
=========
>>> coerce(1, 1.5)
(1.0, 1.5)
>>> coerce(1 + 2j, 1)
((1+2j), (1+0j))
>>> coerce(1.0, 1+3j)
((1+0j), (1+3j))
>>> coerce('foo', 1+3j)
Traceback (most recent call last):
  File "<interactive input>", line 1, in <module>
TypeError: number coercion failed

Example 2
=========
>>> 2 + 4.0        #note that the type coercion is done automatically
6.0
>>> 2 + 4.0
6.0
>>> 1 + 2j+1
(2+2j)

See Also
========
#TODO