==============================
% (String Formatting Operator)
==============================

Description
-----------
Formats the string according to the specified format.

Syntax
------
*%[key][flags][width][.precision][length type]conversion type* % **values**

*%*
    Required. The '%' character, which marks the start of the specifier. 
*key*
    Optional. Mapping key, consisting of a parenthesised sequence of characters (for example, (somename)). 
*flags*
    Optional. Conversion flags, which affect the result of some conversion types.
*width*
    Optional. Minimum field width. If specified as an '*' (asterisk), the actual width is read from the next element of the tuple in values, and the object to convert comes after the minimum field width and optional precision. 
*precision*
    Optional. Precision, given as a '.' (dot) followed by the precision. If specified as '*' (an asterisk), the actual width is read from the next element of the tuple in values, and the value to convert comes after the precision. 
*length type*
    Optional. Length modifier. 
*conversion type*
    Optional. Conversion type. 
**values**
    Required. A number, string or a container with values to substitute for the conversion type.
    
Conversion Flags
----------------
*'#'*
    The value conversion will use the “alternate form” (where defined below).
*'0'*
    The conversion will be zero padded for numeric values.
*'-'*
    The converted value is left adjusted (overrides the '0' conversion if both are given).
*' '*
    (a space) A blank should be left before a positive number (or empty string) produced by a signed conversion.
*'+'*
    A sign character ('+' or '-') will precede the conversion (overrides a “space” flag).
    
A length modifier (h, l, or L) may be present, but is ignored as it is not necessary for Python – so e.g. %ld is identical to %d.

Conversion Types
----------------
*'d'*
    Signed integer decimal.	 
*'i'*
    Signed integer decimal.	 
*'o'*
    Signed octal value.	The alternate form causes a leading zero ('0') to be inserted between left-hand padding and the formatting of the number if the leading character of the result is not already a zero.
*'u'*
    Obsolete type – it is identical to 'd'.	See PEP 237.
*'x' or 'X'*
    Signed hexadecimal.	The alternate form causes a leading '0x' or '0X' (depending on whether the 'x' or 'X' format was used) to be inserted between left-hand padding and the formatting of the number if the leading character of the result is not already a zero.
*'e' or 'E'*
    Floating point exponential format.	The alternate form causes the result to always contain a decimal point, even if no digits follow it.
    
    The precision determines the number of digits after the decimal point and defaults to 6.
*'f' or 'F'*
    Floating point decimal format.	The alternate form causes the result to always contain a decimal point, even if no digits follow it.
    
    The precision determines the number of digits after the decimal point and defaults to 6.
*'g' or 'G'*
    Floating point format. Uses exponential format if exponent is less than -4 or not less than precision, decimal format otherwise.	The alternate form causes the result to always contain a decimal point, and trailing zeroes are not removed as they would otherwise be.
    
    The precision determines the number of significant digits before and after the decimal point and defaults to 6.
*'c'*
    Single character (accepts integer or single character string).	 
*'r'*
    String (converts any Python object using repr()).
    
    The precision determines the maximal number of characters used.
*'s'*
    String (converts any Python object using str()).
    
    If the object or format provided is a unicode string, the resulting string will also be unicode.
    
    The precision determines the maximal number of characters used.
*'%'*
    No argument is converted, results in a '%' character in the result.
    
Remarks
-------
If **format specifier** is a Unicode object, or if any of the objects being converted using the %s conversion are Unicode objects, the result will also be a Unicode object.

If **format specifier** requires a single argument, **values** may be a single non-tuple object. Otherwise, **values** must be a tuple with exactly the number of items specified by the format string, or a single mapping object (for example, a dictionary).

When the right argument is a dictionary (or other mapping type), then the formats in the string **must** include a parenthesised mapping key into that dictionary inserted immediately after the '%' character. The mapping key selects the value to be formatted from the mapping. For example:

>>> print '%(language)s has %(number)03d quote types.' % \
...       {"language": "Python", "number": 2}
Python has 002 quote types.
    
In this case no * specifiers may occur in a format (since they require a sequential parameter list).

Example 1
---------
>>> '%d' % 100  # This Example shows simple substitution.
'100'
>>> '%d' % 0b1111
'15'
>>> "%s" % 'foo'
'foo'
>>> "%s %s" % ('foo', 'bar')
'foo bar'
>>> dct = {'foo': 10, 'bar': 20}
>>> "%(foo)s" % dct
'10'

Example 2
---------
>>> "%x" % 17   # This Example shows usage of # flag (alternate form).  
'11'
>>> "%#x" % 17
'0x11'
>>> "%#X" % 17
'0X11'
    
Example 3
---------
>>> "%d" % 1    # This Example shows usage of zero padding and width flags.
'1'
>>> "%03d" % 1
'001'

Example 4
---------
>>> "%d" % 1    # This Example shows usage of left adjust flag.
'1'
>>> "%-5d" % 1
'1    '
>>> "%0-5d" % 1
'1    '

Example 5
---------
>>> '%d' % 1    # This Example shows usage of space flag.
'1'
>>> '%d' % -1
'-1'
>>> '% d' % 1
' 1'
>>> '% d' % -1
'-1'

Example 6
---------
>>> '%d' % 1    # This Example shows usage of sign flag.
'1'
>>> '%+d' % 1
'+1'
>>> '%+d' % -1
'-1'
>>> '% +d' % -1
'-1'
>>> '% +d' % 1
'+1'

Example 7
---------
>>> '%f' % 3.14     # This Example shows usage of precision modifier.
'3.140000'
>>> '%.1f' % 3.14
'3.1'
>>> '%.2f' % 3.14
'3.14'
>>> '%.3f' % 3.14
'3.140'
    
Example 8
---------
>>> '%i' % 0b1111   # This Example shows how to covert to signed integer decimals.
'15'
>>> '%d' % 0b1111
'15'
>>> '%d' % 10
'10'
>>> '%d' % 3.14
'3'
>>> '%i' % 3.14
'3'
>>> '%i' % -10
'-10'

Example 9
---------
>>> '%x' % 27   # Hex and octal conversions.
'1b'
>>> '%X' % 27
'1B'
>>> '%o' % 27
'33'

Example 10
----------
>>> '%f' % 10   # Float conversions.
'10.000000'
>>> '%F' % 10
'10.000000'
>>> '%g' % 1234567890
'1.23457e+09'
>>> '%G' % 1234567890
'1.23457E+09'
>>> '%e' % 1234567890
'1.234568e+09'
>>> '%E' % 1234567890
'1.234568E+09'

Example 11
----------
>>> 'ABC %c' % 10   # Character and string conversions.
'ABC \n'
>>> 'ABC %c' % 67
'ABC C'
>>> 'ABC %c' % 68
'ABC D'
>>> 'ABC %c' % 'D'
'ABC D'
>>> 'ABC %s' % 68
'ABC 68'
>>> 'ABC %r' % 68
'ABC 68'
