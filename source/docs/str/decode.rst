======
decode
======

Description
----------
Decodes the string using the codec registered for encoding.

Syntax
------
**str**. *decode([encoding[, errors]])*

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
**unicode**

Time Complexity
---------------
#TODO

Example
-------
>>> 'źdźbło'.decode('windows-1250')  # polish word meaning a blade of grass
u'\u0139\u015fd\u0139\u015fb\u0139\u201ao'
>>> 'źdźbło'.decode('ascii', 'strict')
Traceback (most recent call last):
  File "<interactive input>", line 1, in <module>
UnicodeDecodeError: 'ascii' codec can't decode byte 0xc5 in position 0: ordinal not in range(128)
>>> 'źdźbło'.decode('ascii', 'ignore')
u'dbo'
>>> 'źdźbło'.decode('ascii', 'replace')
u'\ufffd\ufffdd\ufffd\ufffdb\ufffd\ufffdo'

See Also
--------
`encode()`_

.. _encode(): ../str/encode.html
