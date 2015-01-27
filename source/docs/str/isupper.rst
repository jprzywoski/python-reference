=======
isupper
=======

Description
----------
Returns a Boolean stating whether the string is in UPPER CASE.

Syntax
------
**str**. *isupper()*

Return Value
------------
**bool**

Time Complexity
---------------
#TODO

Remarks
-------
For 8-bit strings, this method is locale-dependent. Returns **False** if string is empty.

Example
-------
>>> ''.isupper()
False
>>> 'abc123'.isupper()
False
>>> 'abc'.isupper()
False
>>> '123'.isupper()
False
>>> 'Abc Def'.isupper()
False
>>> 'Abc def'.isupper()
False
>>> '!@#'.isupper()
False
>>> '   '.isupper()
False
>>> 'ABC'.isupper()
True 

See Also
--------
`isalnum()`_, `isalpha()`_, `isdigit()`_, `islower()`_, `isspace()`_, `istitle()`_, `isupper()`_

.. _isalnum(): ../str/isalnum.html
.. _isalpha(): ../str/isalpha.html
.. _isdigit(): ../str/isdigit.html
.. _islower(): ../str/islower.html
.. _isspace(): ../str/isspace.html
.. _istitle(): ../str/istitle.html
.. _isupper(): ../str/isupper.html
