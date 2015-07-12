====
str
====
The items of a string are characters. There is no separate character type; a character is represented by a string of one item. Characters represent (at least) 8-bit bytes. The built-in functions chr() and ord() convert between characters and nonnegative integers representing the byte values. Bytes with the values 0-127 usually represent the corresponding ASCII values, but the interpretation of values is up to the program. The string data type is also used to represent arrays of bytes, e.g., to hold data read from a file.

Strings are immutable sequences.

Constructors
====
`str()`_
    Returns a string containing a printable representation of an object.
`x"string" (string designators)`_
    Returns a modified string.
`literal syntax`_
    Initializes a new instance of the **str** type. 

Methods
====

Searching
----
`find`_
    Returns the index of the first occurrence of the string searched for.
`rfind`_
    Returns the index of the last occurrence of the string searched for.
`index`_
    Returns the index of the first occurrence of the string searched for (raises *ValueError* if not found).
`rindex`_
    Returns the index of the last occurrence of the string searched for (raises *ValueError* if not found).
    
Replacing
----
`replace`_
    Returns a copy of the string with a specified substring replaced specified number of times.
`translate`_
    Returns a copy of the string with characters mapped through the given translation table or deleted.

Leading and Trailing Characters
----
    
`lstrip`_
    Returns a copy of the string with leading characters removed.
`rstrip`_
    Returns a copy of the string with trailing characters removed.
`strip`_
    Returns a copy of the string with leading and trailing characters removed.
    
Splitting and Joining
----
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
----
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
----
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
----
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
----
`decode`_
    Decodes the string using the codec registered for encoding.
`encode`_
    Returns an encoded version of the string.
    
Functions
====
`len`_
    Returns an int type specifying number of elements in the collection.
`min`_
    Returns the smallest item from a collection.
`max`_
    Returns the largest item in an iterable or the largest of two or more arguments.
`cmp`_
    Compares two objects and returns an integer according to the outcome.
`sorted`_
    Returns a sorted list from the iterable.
`reversed`_
    Returns a reverse iterator over a sequence.
`all`_
    Returns a Boolean value that indicates whether the collection contains only values that evaluate to True.
`any`_
    Returns a Boolean value that indicates whether the collection contains any values that evaluate to True.
`enumerate`_
    Returns an enumerate object.
`zip`_
    Returns a list of tuples, where the i-th tuple contains the i-th element from each of the argument sequences or iterables.
`chr`_
    Returns a string of one character whose ASCII code is the specified number.
`ord`_
    Returns an integer representing the code of the character.
`unichr`_
    Returns a Unicode character specified by the code.
`format`_
    Returns a formatted string.
    
Operators
====
`% (string formatting)`_
    Formats the string according to the specified format.
`[] (index operator)`_
    Gives access to a sequence's element.
`[::] (slicing)`_
    Gives access to a specified range of sequence's elements.
`+ (concatenation)`_
    Returns a concatenation of two sequences.
`* (multiple concatenation)`_
    Returns a sequence self-concatenated specified amount of times.
    
Misc
====
`Escape Characters`_
    List of valid escape characters.
`ASCII Table (0 - 127)`_
    Basic character set.

    
.. _str(): ../functions/str.html
.. _literal syntax: literals.html
.. _% (String Formatting Operator): formatting.html
.. _x"string" (String Designators): designators.html
.. _Escape Characters: escapes.html
.. _[] (index operator): ../brackets/indexing.html
.. _[::] (slicing): ../brackets/slicing.html
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
.. _ASCII Table (0 - 127): ascii.html
.. _enumerate: ../functions/enumerate.html
.. _len: ../functions/len.html
.. _reversed: ../functions/reversed.html
.. _sorted: ../functions/sorted.html
.. _sum: ../functions/sum.html
.. _zip: ../functions/zip.html
.. _cmp: ../functions/cmp.html
.. _max: ../functions/max.html
.. _min: ../functions/min.html
.. _all: ../functions/all.html
.. _any: ../functions/any.html
.. _+ (concatenation): ../operators/concatenation.html
.. _* (multiple concatenation): ../operators/multiple_concatenation.html
.. _chr: ../functions/chr.html
.. _ord: ../functions/ord.html
.. _unichr: ../functions/unichr.html
.. _format: ../functions/format.html
