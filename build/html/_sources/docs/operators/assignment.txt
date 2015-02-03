============
= Assignment
============

Description
===========
Assigns the result of the right hand side operand to the left hand side operand.

Syntax
======
A = B

Remarks
=======
The assignment operator assigns a value to a variable.

a = 5;

This statement assigns the integer value 5 to the variable a. The part at the left of the assignment operator (=) is
known as the lvalue (left value) and the right one as the rvalue (right value). The lvalue has to be a variable
whereas the rvalue can be either a constant, a variable, the result of an operation or any combination of these.
The most important rule when assigning is the right-to-left rule: The assignment operation always takes place from
right to left, and never the other way:

This statement assigns to variable a (the lvalue) the value contained in variable b (the rvalue). The value that was
stored until this moment in a is not considered at all in this operation, and in fact that value is lost.

The following expression is also valid in C++:

a = b = c = 5;

It assigns 5 to the all the three variables: a, b and c.

A, b = 10, 12


Example
=======
>>> a = 0
>>> b = 1
>>> c = a + b
>>> c
1
>>> foo = 'bar'