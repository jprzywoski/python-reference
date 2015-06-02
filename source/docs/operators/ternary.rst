=======================================
if else conditional operator
=======================================

Description
===========
Returns either value depending on the result of a Boolean expression.

Syntax
======
**A if expression else B**

*A*
    The value for the entire conditional expression if the condition is True.
*expression*
    The condition that evaluates to a Boolean. 
*B*
    The value for the entire conditional expression if the condition is False.

Return Value
============
The same as passed to the expression.

Time Complexity
============
#TODO

Remarks
=======
Python's conditional operator is similar to the if else statement. It is also called a ternary operator since it takes three operands (as opposed to binary operands like +, - or unary ones like ~).

Example 1
=======
>>> 1 if True else 0
1
>>> 1 if False else 0
0

Example 2
====
>>> rating = 100
>>> 'good' if rating > 80 else 'bad'
'good'

The above expression returns 'good' if rating is greater than 80 and 'bad' otherwise.

Note that conditional operator does not allow the use of statements:

Example 3
====
>>> print 'good' if rating > 80 else print 'bad'
  File "<interactive input>", line 1
    print 'good' if rating > 80 else print 'bad'
                                         ^
SyntaxError: invalid syntax

See also
========
#TODO