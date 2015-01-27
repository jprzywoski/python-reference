======
encode
======

Description
----------
Returns an encoded version of the string.

Syntax
------
**str**. *encode([encoding[, errors]])*

*encoding*
    Optional. The desired encoding. Defaults to the default string encoding. See codecs module for a full list.
*errors*
    Optional. *errors* may be given to set a different error handling scheme.
    
Typical *errors* values:

*'strict'*
    Raise ValueError (or a subclass); this is the default. 
*'ignore'*
    Ignore the character and continue with the next. 
*'replace'*
    Replace with a suitable replacement character 
Other possible values are any other name registered via codecs.register_error(), see section Codec Base Classes.

Return Value
------------
**str**

Time Complexity
---------------
#TODO

Example
-------
>>> 'foo'.encode()
'foo'
>>> 'foo'.encode('windows-1250', 'strict')
'foo'
>>> 'foo'.encode('windows-1250', 'ignore')
'foo'
>>> 'foo'.encode('windows-1250', 'replace')
'foo'
>>> 'foo'.encode('windows-1250', 'xmlcharrefreplace')
'foo'
>>> 'foo'.encode('windows-1250', 'backslashreplace')
'foo'

See Also
--------
`decode()`_

.. _decode(): ../str/decode.html
