===
str
===

`Overview`_

Constructors
------------
`str()`_
    
`Literal Syntax`_

Misc
----
`String Designators`_
    
`% (String Formatting Operator)`_
    Formats the string according to the specified format.
`Escape Charcters`_
    
Methods
-------

Searching
_________
`find`_
    Returns the index of the first occurrence of the string searched for.
`rfind`_
    Returns the index of the last occurrence of the string searched for.
`index`_
    Returns the index of the first occurrence of the string searched for (raises *ValueError* if not found).
`rindex`_
    Returns the index of the last occurrence of the string searched for (raises *ValueError* if not found).
    
Replacing
_________
`replace`_
    Returns a copy of the string with a specified substring replaced specified number of times.
`translate`_
    Returns a copy of the string with characters mapped through the given translation table or deleted.

Leading and Trailing Characters
_______________________________
    
`lstrip`_
    Returns a copy of the string with leading characters removed.
`rstrip`_
    Returns a copy of the string with trailing characters removed.
`strip`_
    Returns a copy of the string with leading and trailing characters removed.
    
Splitting and Joining
____________________
`split`_
    Returns a list of the words in the string, separated by the delimiter string.
`rsplit`_
    Returns a list of the words in the string, separated by the delimiter string (starting from right).
`partition`_
    Returns a tuple containing the first part of the string split by the specified separator, the separator itself and the other part of the string.
`rpartition`_
    Returns a tuple containing the first part of the string split by the specified separator, the separator itself and the other part of the string (starting from right).
`splitlines`_
    Returns a list of the lines in the string, breaking at line boundaries.
`join`_
    Returns a string made from the elements of an iterable.

Changing Case
_____________
`upper`_
    Returns a copy of the string in UPPER CASE.
`lower`_
    Returns a copy of the string in lower case.
`capitalize`_
    Returns a copy of the string in Capital case.
`title`_
    Returns a copy of the string in Title Case.
`swapcase`_
    Returns a copy of the string with case swapped.

Information
___________
`count`_
    Returns the number of non-overlapping occurrences of a substring in the searched string.
`startswith`_
    Returns a Boolean stating whether a string starts with the specified prefix.
`endswith`_
    Returns a Boolean stating whether a string ends with the specified suffix.
`isalnum`_
    Returns a Boolean stating whether the string contains only letters and digits.
`isalpha`_
    Returns a Boolean stating whether the string contains only letters.
`isdigit`_
    Returns a Boolean stating whether the string contains only digits.
`islower`_
    Returns a Boolean stating whether the string is in lower case.
`isspace`_
    Returns a Boolean stating whether the string contains only whitespace characters.
`istitle`_
    Returns a Boolean stating whether the string is in Title case.
`isupper`_
    Returns a Boolean stating whether the string is in UPPER CASE.
    
Formatting
__________
`ljust`_
    Returns the string left justified in a string of specified length.
`rjust`_
    Returns the string right justified in a string of specified length.
`center`_
    Returns the string centered in a string of specified length.
`zfill`_
    Returns the numeric string left filled with zeros in a string of specified length.
`expandtabs`_
    Returns a copy of the string where all tab characters were replaced by spaces.
`format`_
    Returns a formatted version of the string.
    
Encodings
_________
`decode`_
    Decodes the string using the codec registered for encoding.
`encode`_
    Returns an encoded version of the string.

.. _Overview: ../str/overview.html
.. _% (String Formatting Operator): ../str/formatting.html
.. _find: ../str/find.html
.. _rfind: ../str/rfind.html
.. _index: ../str/strindex.html
.. _rindex: ../str/rinddex.html
.. _translate: ../str/translate.html
.. _replace: ../str/replace.html
.. _upper: ../str/upper.html
.. _lower: ../str/lower.html
.. _capitalize: ../str/capitalize.html
.. _title: ../str/title.html
.. _swapcase: ../str/swapcase.html
.. _lstrip: ../str/lstrip.html
.. _rstrip: ../str/rstrip.html
.. _strip: ../str/strip.html
.. _split: ../str/split.html
.. _rsplit: ../str/rsplit.html
.. _partition: ../str/partition.html
.. _rpartition: ../str/rpartition.html
.. _splitlines: ../str/splitlines.html
.. _join: ../str/join.html
.. _startswith: ../str/startswith.html
.. _endswith: ../str/endswith.html
.. _count: ../str/count.html
.. _isalnum: ../str/isalnum.html
.. _isalpha: ../str/isalpha.html
.. _isdigit: ../str/isdigit.html
.. _islower: ../str/islower.html
.. _isspace: ../str/isspace.html
.. _istitle: ../str/istitle.html
.. _isupper: ../str/isupper.html
.. _ljust: ../str/ljust.html
.. _center: ../str/center.html
.. _rjust: ../str/rjust.html
.. _zfill: ../str/zfill.html
.. _expandtabs: ../str/expandtabs.html
.. _format: ../str/format.html
.. _decode: ../str/decode.html
.. _encode: ../str/encode.html

