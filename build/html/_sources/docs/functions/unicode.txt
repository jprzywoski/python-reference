=======
unicode
=======

Description
===========
Returns the Unicode string version of object.

Syntax
======
**unicode** *(object='')*
**unicode** *(object[, encoding[, errors]])*

*object*
	Required. An object to be converted to string.
*encoding*
	Optional. String encoding.
*errors*
	Optional. Errors.

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
If encoding and/or errors are given, unicode() will decode the object which can either be an 8-bit string or a character buffer using the codec for encoding. The encoding parameter is a string giving the name of an encoding; if the encoding is not known, LookupError is raised. Error handling is done according to errors; this specifies the treatment of characters which are invalid in the input encoding. If errors is 'strict' (the default), a ValueError is raised on errors, while a value of 'ignore' causes errors to be silently ignored, and a value of 'replace' causes the official Unicode replacement character, U+FFFD, to be used to replace input characters which cannot be decoded. See also the codecs module.

If no optional parameters are given, unicode() will mimic the behaviour of str() except that it returns Unicode strings instead of 8-bit strings. More precisely, if object is a Unicode string or subclass it will return that Unicode string without any additional decoding applied.

For objects which provide a __unicode__() method, it will call this method without arguments to create a Unicode string. For all other objects, the 8-bit string version or representation is requested and then converted to a Unicode string using the codec for the default encoding in 'strict' mode.

Example 1
=========
>>> unicode(10.25)
u'10.25'
>>> unicode((1, 2))
u'(1, 2)'
>>> unicode([1, 2])
u'[1, 2]'
>>> unicode({1, 2})
u'set([1, 2])'
>>> unicode({'a': 1, 'b': 2})
u"{'a': 1, 'b': 2}"
>>> unicode('foobar')
u'foobar'

Example 2
=========
>>> unicode('źdźbło', 'windows-1250')
u'\u0139\u013dd\u0139\u015fb\u0139\u201ao'

Example 3
=========
>>> unicode('źdźbło', 'ascii', 'ignore')
u'dbo'
>>> unicode('źdźbło', 'ascii', 'strict')
Traceback (most recent call last):
  File "<interactive input>", line 1, in <module>
UnicodeDecodeError: 'ascii' codec can't decode byte 0xc5 in position 0: ordinal not in range(128)
>>> unicode('źdźbło', 'ascii', 'replace')
u'\ufffd\ufffdd\ufffd\ufffdb\ufffd\ufffdo'

See Also
========
#TODO