=======
isspace
=======

Description
----------
Returns a Boolean stating whether the string contains only whitespace characters.

Syntax
------
**str**. *isspace()*

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
>>> ''.isspace()
False
>>> 'abc123'.isspace()
False
>>> 'abc'.isspace()
False
>>> '123'.isspace()
False
>>> 'Abc'.isspace()
False
>>> '!@#'.isspace()
False
>>> '   '.isspace()
True
>>> 'ABC'.isspace()
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
