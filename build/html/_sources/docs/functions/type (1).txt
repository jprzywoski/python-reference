========
type (1)
========

Description
===========
Returns the type of an object (constructor name).

Syntax
======
**type** *(object)*

*object*
	Required. An object which type constructor is to be returned.

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
The isinstance() built-in function is recommended for testing the type of an object. See type() (2) for three arguments syntax.

Example 1
=========
>>> type(2147483647)
<type 'int'>
>>> type(2147483648)
<type 'long'>
>>> type(3.14)
<type 'float'>
>>> type(3 + 2j)
<type 'complex'>

Example 2
=========
>>> type('foobar')
<type 'str'>
>>> type(u'foobar')
<type 'unicode'>
>>> type((1, 2))
<type 'tuple'>
>>> type([1, 2])
<type 'list'>
>>> type({'a': 1, 'b': 2})
<type 'dict'>
>>> type({1, 2})
<type 'set'>

See Also
========
#TODO