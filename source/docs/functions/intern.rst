======
intern
======

Description
===========
Enters the string into interned strings table (if not already there).

Syntax
======
**intern** *(string)*

*string*
	Required. The string you want to intern.

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
By using intern you ensure that you never create two string objects that have the same value - when you request the creation of a second string object with the same value as an existing string object, you receive a reference to the pre-existing string object. This way, you are saving memory. Also, string objects comparison is now very efficient because it is carried out by comparing the memory addresses of the two string objects instead of their content.

Essentially intern looks up (or stores if not present) the string in a collection of interned strings, so all interned instances will share the same identity. You trade the one-time cost of looking up this string for faster comparisons (the compare can return True after just checking for identity, rather than having to compare each character), and reduced memory usage.

However, python will automatically intern strings that are small, or look like identifiers, so you may find you get no improvement because your strings are already being interned behind the scenes.

Example 1
=========
>>> f = 'foobar'
>>> b = 'foobar'
>>> f == b
True
>>> f is b
True
>>> b = 'foobar qwertyuiop'
>>> f = 'foobar qwertyuiop'
>>> b is f
False

Example 2
=========
>>> a = intern('spam foobar snafu')
>>> b = 'spam foobar snafu'
>>> a is b
False
>>> b = intern('spam foobar snafu')
>>> a is b
True

See Also
========
#TODO