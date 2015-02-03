=====
print
=====

Description
===========
Returns a printed representation of the objects.

Syntax
======
**print** *(*objects, sep=' ', end='\n', file=sys.stdout)*

*objects*
	Optional. Objects to be printed.
*sep*
	Optional. A string printed between objects. Keyword argument.
*end*
	Optional. A string appended to the end of the statement. Keyword argument.
*file*
	Optional. An object with write(string) method. Keyword argument.

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
All non-keyword arguments are converted to strings like str() does and written to the stream, separated by sep and followed by end. Both sep and end must be strings; they can also be None, which means to use the default values. If no objects are given, print() will just write end.

The file argument must be an object with a write(string) method; if it is not present or None, sys.stdout will be used. Output buffering is determined by file. Use file.flush() to ensure, for instance, immediate appearance on a screen.

Note
====
This function is not normally available as a built-in since the name print is recognized as the print statement. To disable the statement and use the print() function, use this future statement at the top of your module:

>>> from __future__ import print_function

Example 1
=========
>>> from __future__ import print_function
>>> print('a', 'b')
a b

Example 2
=========
>>> print(1, 2, 3, sep='|')
1|2|3
>>> print('foobar snafu', end='|')
foobar snafu|

Example 3
=========
>>> print('foobar', file=open(r'C:\test.txt', "w"))
>>> open(r'C:\test.txt', "r").read()
'foobar\n'

See Also
========
#TODO