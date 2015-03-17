====
send
====

Description
===========
Resumes the execution and “sends” a value into the generator function.

Syntax
======
**generator.** *send(value)*

*value*
    Required. The value of the item to be sent.

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
The value argument becomes the result of the current yield expression. The send() method returns the next value yielded by the generator, or raises StopIteration if the generator exits without yielding another value. When send() is called to start the generator, it must be called with None as the argument, because there is no yield expression that could receive the value.

Example
=========
>>> def gen(n=None):
...     for i in range(n):
...         n = yield n
...         
>>> g = gen(3)
>>> g.next()
3
>>> g.next()
>>> g.send(10)
10
>>> g.send(10)
Traceback (most recent call last):
  File "<interactive input>", line 1, in <module>
StopIteration

See Also
========
#TODO
