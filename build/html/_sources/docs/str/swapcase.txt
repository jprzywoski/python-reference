========
swapcase
========

Description
----------
Returns a copy of the string with case swapped.

Syntax
------
**str**. *swapcase()*

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
>>> 'foo'
'foo'
>>> 'foo'.swapcase()
'FOO'
>>> 'Foo'.swapcase()
'fOO'
>>> 'fOo'.swapcase()
'FoO'
>>> '123'.swapcase()
'123'
>>> '!@#'.swapcase()
'!@#'
>>> '   '.swapcase()
'   '

See Also
--------
`upper`_

`lower`_

`capitalize`_

`title`_


.. _upper: ../bd_strings/upper.html
.. _lower: ../bd_strings/lower.html
.. _capitalize: ../bd_strings/capitalize.html
.. _title: ../bd_strings/title.html
.. _swapcase: ../bd_strings/swapcase.html