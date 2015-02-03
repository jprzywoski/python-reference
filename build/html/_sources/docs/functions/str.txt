===
str
===

Description
===========
Returns a string containing a printable representation of an object.

Syntax
======
**str** *(object)*

*object*
	Optional. Any object. If omitted an empty string is returned.

Return Value
============
**str**

Time Complexity
============
#TODO

Remarks
=======
Returns a string containing a nicely printable representation of an object. For strings, this returns the string itself. The difference with repr(object) is that str(object) does not always attempt to return a string that is acceptable to eval(); its goal is to return a printable string.

See also unicode().

Example 1
=========
>>> str()
''
>>> str(10)
'10'
>>> str([1, 2])
'[1, 2]'
>>> str((1, 2))
'(1, 2)'
>>> str({'a': 1, 'b': 2})
"{'a': 1, 'b': 2}"
>>> str({1, 2})
'set([1, 2])'

Example 2
=========
>>> str('foobar')
'foobar'
>>> str("""foobar""")
'foobar'
>>> str("foobar")
'foobar'

Example 3
=========
>>> print str('foobar')
foobar
>>> print repr('foobar')
'foobar'
>>> str('foobar') == repr('foobar')
False

See Also
========
#TODO