============
= Assignment
============

Description
===========
Assigns a value to a variable(s).

Syntax
======
**A = B**

*A*
    Any valid object.
*B*
    Any valid object.
    
Return Value
============
According to coercion rules.

Time Complexity
============
#TODO

Remarks
=======
Assignment operation always works from right to left. The object that was referenced by the variable prior to the assignment is now dereferenced.

Example 1
====
>>> a = 10
>>> a = 5
>>> a
5

Multiple assignment also follows the right-to-left rule. Consider the following example:

Example 2
====
>>> a = b = c = 10
>>> a
10
>>> b
10
>>> c
10

First the integer 10 is assigned to the variable c, then the value of c (10) is assigned to b and b is assigned to a. After evaluating this expression all the variables are referencing the same object - integer 10.

Another case of assignment is a multi-variable assignment. Consider the following example:

Example 3
====
>>> a, b, c = 1, 2, 3  # <- this is a tuple
>>> a
1
>>> b
2
>>> c
3

Following right-to-left rule a tuple containing (1, 2, 3) is created, then it is iterated over and its consequent values are assigned to the comma separated list of variables on the left.

This syntax can be used to swap the values of two variables:

Example 4
====
>>> a = 0
>>> b = 1
>>> a, b = b, a
>>> a
1
>>> b
0

Another common use is when we want to assign new values based on existing values:

Example 5a
====
>>> a = 10
>>> b = 5
>>> a, b = a + b, a * b
>>> a
15
>>> b
50

this is different than:

Example 5b
====
>>> a = 10
>>> b = 5
>>> a = a + b
>>> b = a * b
>>> a
15
>>> b
75

See Also
========
#TODO
