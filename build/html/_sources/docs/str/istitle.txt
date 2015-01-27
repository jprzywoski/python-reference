=======
istitle
=======

Description
----------
Returns a Boolean stating whether the string is in Title case.

Syntax
------
**str**. *istitle()*

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
>>> ''.istitle()
False
>>> 'abc123'.istitle()
False
>>> 'abc'.istitle()
False
>>> '123'.istitle()
False
>>> 'Abc Def'.istitle()
True
>>> 'Abc def'.istitle()
False 
>>> '!@#'.istitle()
False
>>> '   '.istitle()
False
>>> 'ABC'.istitle()
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
