====
next
====

Description
===========
Starts the execution of a generator function or resumes it at the last executed yield expression.

Syntax
======
**generator.** *next()*

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
When a generator function is resumed with a next() method, the current yield expression always evaluates to None. The execution then continues to the next yield expression, where the generator is suspended again, and the value of the expression_list is returned to next()'s caller. If the generator exits without yielding another value, a StopIteration exception is raised.

Example 1
=========
>>> def gen():
...     yield 1
...     yield 2
...     yield 3
...     
>>> g = gen()
>>> g.next()
1
>>> g.next()
2
>>> g.next()
3
>>> g.next()
Traceback (most recent call last):
  File "<interactive input>", line 1, in <module>
StopIteration

See Also
========
#TODO
