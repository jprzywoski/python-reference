=====
title
=====

Description
----------
Returns a copy of the string in Title Case.

Syntax
------
**str**. *title()*

Return Value
------------
**str**

Time Complexity
---------------
#TODO

Remarks
-------
The algorithm uses a simple language-independent definition of a word as groups of consecutive letters. The definition works in many contexts but it means that apostrophes in contractions and possessives form word boundaries, which may not be the desired result:

Example 1
---------
>>> "they're bill's friends from the UK".title()
"They'Re Bill'S Friends From The Uk"

A workaround for apostrophes can be constructed using regular expressions:

Example 2
---------
>>> import re
>>> def titlecase(s):
...     return re.sub(r"[A-Za-z]+('[A-Za-z]+)?",
...         lambda mo: mo.group(0)[0].upper() +
...             mo.group(0)[1:].lower(), s)
...             
>>> titlecase("they're bill's friends.")
"They're Bill's Friends."

For 8-bit strings, this method is locale-dependent.

See Also
--------
`upper`_

`lower`_

`capitalize`_

`swapcase`_

.. _upper: ../bd_strings/upper.html
.. _lower: ../bd_strings/lower.html
.. _capitalize: ../bd_strings/capitalize.html
.. _title: ../bd_strings/title.html
.. _swapcase: ../bd_strings/swapcase.html