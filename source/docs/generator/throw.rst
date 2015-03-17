====
throw
====

Description
===========
Raises a specified exception at the point where generator was paused, and returns the next value yielded by the generator function.

Syntax
======
**generator.** *throw(type[, value[, traceback]])*

*type*
    Required. Type of execpetion.
*value*
    Optional. The value of the error.
*traceback*
    Optional. A traceback object.

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
If the generator exits without yielding another value, a StopIteration exception is raised. If the generator function does not catch the passed-in exception, or raises a different exception, then that exception propagates to the caller.

Example 1
====
>>> # this example shows how to use throw method
>>> g = (n**2 for n in (1, 2, 3))
>>> g.throw(TypeError)
Traceback (most recent call last):
  File "<interactive input>", line 1, in <module>
  File "<interactive input>", line 1, in <genexpr>
TypeError

Example 2
====
>>> # this example shows how to use throw method with value argument
>>> g = (n**2 for n in (1, 2, 3))
>>> g.throw(TypeError, 'ERROR')
Traceback (most recent call last):
  File "<interactive input>", line 1, in <module>
  File "<interactive input>", line 1, in <genexpr>
TypeError: ERROR

See Also
========
#TODO
