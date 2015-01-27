=======
isdigit
=======

Description
----------
Returns a Boolean stating whether the string contains only digits.

Syntax
------
**str**. *isdigit()*

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
>>> ''.isdigit()
False
>>> 'abc123'.isdigit()
False
>>> 'abc'.isdigit()
False
>>> '123'.isdigit()
True
>>> 'Abc'.isdigit()
False
>>> '!@#'.isdigit()
False
>>> '   '.isdigit()
False
>>> 'ABC'.isdigit()
False 

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
