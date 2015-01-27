=====
lower
=====

Description
----------
Returns a copy of the string in lower case.

Syntax
------
**str**. *lower()*

Return Value
------------
**str**

Time Complexity
---------------
#TODO

Remarks
-------
For 8-bit strings, this method is locale-dependent.

Example
-------
>>> 'foo'.lower()
'foo'
>>> 'Foo'.lower()
'foo'
>>> 'FOO'.lower()
'foo'
>>> '123'.lower()
'123'
>>> ''.lower()
''
>>> '   '.lower()
'   '
>>> '!@#'.lower()
'!@#'

See Also
--------
`upper`_

`capitalize`_

`title`_

`swapcase`_

.. _upper: ../bd_strings/upper.html
.. _lower: ../bd_strings/lower.html
.. _capitalize: ../bd_strings/capitalize.html
.. _title: ../bd_strings/title.html
.. _swapcase: ../bd_strings/swapcase.html