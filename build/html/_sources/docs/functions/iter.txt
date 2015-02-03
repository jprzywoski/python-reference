====
iter
====

Description
===========
Returns an iterator object.

Syntax
======
**iter** *(object, [sentinel])*

*object*
	Required. An iterable sequence.
*sentinel*
	Optional. If used object must be callable.

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
The first argument is interpreted very differently depending on the presence of the second argument. Without a second argument, object must be a collection object which supports the iteration protocol (the __iter__() method), or it must support the sequence protocol (the __getitem__() method with integer arguments starting at 0). If it does not support either of those protocols, TypeError is raised. If the second argument, sentinel, is given, then o must be a callable object. The iterator created in this case will call o with no arguments for each call to its next() method; if the value returned is equal to sentinel, StopIteration will be raised, otherwise the value will be returned.

Example 1
=========
>>> i = iter([1, 2, 3])
>>> i.next()
1
>>> i.next()
2
>>> i.next()
3
>>> i.next()
Traceback (most recent call last):
  File "<interactive input>", line 1, in <module>
StopIteration

Example 2
=========
>>> # The following example reads a file until the readline() method returns an empty string
>>> with open(r'C:\alice_in_wonderland.txt') as fp:
...     for line in iter(fp.readline, ''):
...         print line[0]

See Also
========
#TODO
