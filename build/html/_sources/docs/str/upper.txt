=====
upper
=====

Description
----------
Returns a copy of the string in UPPER CASE.

Syntax
------
**str**. *upper()*

Return Value
------------
**str**

Time Complexity
---------------
#TODO

Remarks
-------
Note that *s.upper().isupper()* might be **False** if *s* contains uncased characters or if the Unicode category of the resulting character(s) is not "Lu" (Letter, uppercase), but e.g. "Lt" (Letter, titlecase).

For 8-bit strings, this method is locale-dependent.

Example
-------
>>> 'abc'.upper()
'ABC'
>>> 'ABC'.upper()
'ABC'
>>> 'Abc'.upper()
'ABC'
>>> '123'.upper()
'123'
>>> '!@#'.upper()
'!@#'
>>> ' '.upper()
' '
>>> ''.upper()
''

See Also
--------
`lower`_

`capitalize`_

`title`_

`swapcase`_

.. _upper: ../bd_strings/upper.html
.. _lower: ../bd_strings/lower.html
.. _capitalize: ../bd_strings/capitalize.html
.. _title: ../bd_strings/title.html
.. _swapcase: ../bd_strings/swapcase.html