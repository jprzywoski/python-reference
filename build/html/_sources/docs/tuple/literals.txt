==============
Literal Syntax
==============

Tuples can be initialized using separating multiple expression with a comma ','.

Example 1
=========
>>> t = 'A', 'B'
>>> t
('A', 'B')

However, tuples should always be created using parentheses.

Example 2
=========
>>> t = (1 , 2, 3)
>>> t
(1, 2, 3)

Not using parentheses can cause problems due to the operator precedence rules. Consider the following example using sequence concatenation:

Example 3
=========
>>> (0, 1) + (2, 3)  # this is the way it was intended
(0, 1, 2, 3)
>>> 0, 1 + (2, 3)    # too ambiguous for the interpreter 
Traceback (most recent call last):
  File "<interactive input>", line 1, in <module>
TypeError: unsupported operand type(s) for +: 'int' and 'tuple'



