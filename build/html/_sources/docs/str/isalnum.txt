=======
isalnum
=======

Description
----------
Returns a Boolean stating whether the string contains only letters and digits.

Syntax
------
**str**. *isalnum()*

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
>>> ''.isalnum()
False
>>> 'abc123'.isalnum()
True
>>> 'abc'.isalnum()
True
>>> '123'.isalnum()
True
>>> 'Abc'.isalnum()
True
>>> '!@#'.isalnum()
False
>>> '   '.isalnum()
False
>>> 'ABC'.isalnum()
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
