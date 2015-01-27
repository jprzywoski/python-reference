=======
isalpha
=======

Description
----------
Returns a Boolean stating whether the string contains only letters.

Syntax
------
**str**. *isalpha()*

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
>>> ''.isalpha()
False
>>> 'abc123'.isalpha()
False
>>> 'abc'.isalpha()
True
>>> '123'.isalpha()
False
>>> 'Abc'.isalpha()
True
>>> '!@#'.isalpha()
False
>>> '   '.isalpha()
False
>>> 'ABC'.isalpha()
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
