====
close
====

Description
===========
Raises a GeneratorExit at the point where the generator function was paused.

Syntax
======
**generator.** *close()*

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
If the generator function then raises StopIteration (by exiting normally, or due to already being closed) or GeneratorExit (by not catching the exception), close returns to its caller. If the generator yields a value, a RuntimeError is raised. If the generator raises any other exception, it is propagated to the caller. close() does nothing if the generator has already exited due to an exception or normal exit.

Example
====
>>> g = (n**2 for n in (1, 2, 3))
>>> g.next()
1
>>> g.close()
>>> g.next()
Traceback (most recent call last):
  File "<interactive input>", line 1, in <module>
StopIteration

See Also
========
#TODO
