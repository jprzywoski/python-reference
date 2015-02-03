==============
Literal Syntax
==============

Sets can be initialized by enclosing set elements in squiggly brackets {}.

Example 1
=========
>>> s = {True, 3.14, "ABC"}
>>> s
set([True, 3.14, 'ABC'])

Any duplicated elements are discarded during set creation. This can be useful to extract unique values from an array.

Example 2
=========
>>> s = {0, 0, 1}
>>> s
set([0, 1])

Sets cannot contain mutable types.

Example 3
=========
>>> s = {[0, 1], [1, 0]}
Traceback (most recent call last):
  File "<interactive input>", line 1, in <module>
TypeError: unhashable type: 'list'

