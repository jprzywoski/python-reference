====
repr
====

Description
===========
Returns a string containing a printable representation of an object.

Syntax
======
**repr** *(object)*

*object*
	Required. A valid Python object.

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
The returned value is the same value yielded by conversions (reverse quotes). It is sometimes useful to be able to access this operation as an ordinary function. For many types, this function makes an attempt to return a string that would yield an object with the same value when passed to eval(), otherwise the representation is a string enclosed in angle brackets that contains the name of the type of the object together with additional information often including the name and address of the object. A class can control what this function returns for its instances by defining a __repr__() method.
See also str().

Example 1
=========
>>> repr(1)
'1'
>>> repr([1, 2])
'[1, 2]'
>>> repr({'a': 1, 'b': 2})
"{'a': 1, 'b': 2}"

Example 2
=========
>>> class Foo:
...     pass
...
>>> repr(Foo())
'<__main__.Foo instance at 0x02C19FA8>'
>>>
>>> class Bar:
...     def __repr__(self):
...         return 'bar'
...
>>> repr(Bar())
'bar'

Example 3
=========
>>> repr('hello')
"'hello'"
>>> repr("hello")
"'hello'"
>>> repr("""hello""")
"'hello'"
>>> repr('hello')
"'hello'"

See Also
========
#TODO