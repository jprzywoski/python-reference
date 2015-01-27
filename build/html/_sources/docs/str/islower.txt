=======
islower
=======

Description
----------
Returns a Boolean stating whether the string is in lower case.

Syntax
------
**str**. *islower()*

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
>>> ''.islower()
False
>>> 'abc123'.islower()
True
>>> 'abc'.islower()
True
>>> '123'.islower()
False
>>> 'Abc'.islower()
False
>>> '!@#'.islower()
False
>>> '   '.islower()
False
>>> 'ABC'.islower()
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
