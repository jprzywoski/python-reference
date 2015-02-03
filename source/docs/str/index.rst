===
str
===

The items of a string are characters. There is no separate character type; a character is represented by a string of one item. Characters represent (at least) 8-bit bytes. The built-in functions chr() and ord() convert between characters and nonnegative integers representing the byte values. Bytes with the values 0-127 usually represent the corresponding ASCII values, but the interpretation of values is up to the program. The string data type is also used to represent arrays of bytes, e.g., to hold data read from a file.

Strings are immutable sequences.

Constructors
------------
`str()`_
    Returns a string containing a printable representation of an object.
`literal syntax`_

Misc
----
`..."" (String Designators)`_
    Returns a modified string.
`% (String Formatting Operator)`_
    Formats the string according to the specified format.
`Escape Characters`_
    
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

    
.. _str(): ../functions/str.html
.. _literal syntax: literals.html
.. _% (String Formatting Operator): formatting.html
.. _..."" (String Designators): designators.html
.. _Escape Characters: escapes.html
.. _find: find.html
.. _rfind: rfind.html
.. _index: strindex.html
.. _rindex: rinddex.html
.. _translate: translate.html
.. _replace: replace.html
.. _upper: upper.html
.. _lower: lower.html
.. _capitalize: capitalize.html
.. _title: title.html
.. _swapcase: swapcase.html
.. _lstrip: lstrip.html
.. _rstrip: rstrip.html
.. _strip: strip.html
.. _split: split.html
.. _rsplit: rsplit.html
.. _partition: partition.html
.. _rpartition: rpartition.html
.. _splitlines: splitlines.html
.. _join: join.html
.. _startswith: startswith.html
.. _endswith: endswith.html
.. _count: count.html
.. _isalnum: isalnum.html
.. _isalpha: isalpha.html
.. _isdigit: isdigit.html
.. _islower: islower.html
.. _isspace: isspace.html
.. _istitle: istitle.html
.. _isupper: isupper.html
.. _ljust: ljust.html
.. _center: center.html
.. _rjust: rjust.html
.. _zfill: zfill.html
.. _expandtabs: expandtabs.html
.. _format: format.html
.. _decode: decode.html
.. _encode: encode.html

