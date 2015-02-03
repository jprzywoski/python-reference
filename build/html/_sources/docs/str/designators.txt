======
...""
======

Description
===========
Returns a modified string.

Syntax
======
*[designator]string*

*r | R*
    Raw string. Uses different rules for interpreting backslash escape sequences.
*u | U*
    Unicode string.
*b | B*
    Alias for bytes type; ignored in Python 2; it indicates that the literal should become a bytes literal in Python 3 (e.g. when code is automatically converted with 2to3)
*Ur | UR | Ur | uR*
    Raw Unicode.
*br | Br | bR | BR*
    Raw bytes (see above).

Example 1
=========
>>> r'AB\nCD'
'AB\\nCD'
>>> 'AB\nCD'
'AB\nCD'

Example 2
=========
>>> u'ABCD' 
u'ABCD'
>>> b'ABCD'
'ABCD'

