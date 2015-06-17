======
format
======

Description
----------
Returns a formatted version of the string.

Syntax
------
**str**. *format(*args, **kwargs)*

*args*
    Required. Format strings.
*kwargs*
    Optional. Format strings.

Replacement field can contain format specification in general form:

**[[fill]align][sign][#][0][width][,][.precision][type]**

fill
____
If a valid align value is specified, it can be preceded by a fill character that can be any character and defaults to a space if omitted.

allign
______
*'<'*
    Forces the field to be left-aligned within the available space (this is the default for most objects).
*'>'*
    Forces the field to be right-aligned within the available space (this is the default for numbers).
*'='*
    Forces the padding to be placed after the sign (if any) but before the digits. This is used for printing fields in the form ‘+000000120’. This alignment option is only valid for numeric types.
*'^'*
    Forces the field to be centered within the available space.
    
sign
____
*'+'*
    Indicates that a sign should be used for both positive as well as negative numbers.
*'-'*
    indicates that a sign should be used only for negative numbers (this is the default behavior).
*‘ ‘*
    (space)	indicates that a leading space should be used on positive numbers, and a minus sign on negative numbers.
*‘#’*
    The '#' option is only valid for integers, and only for binary, octal, or hexadecimal output. If present, it specifies that the output will be prefixed by '0b', '0o', or '0x', respectively.
*‘,’*
    The ',' option signals the use of a comma for a thousands separator. For a locale aware separator, use the 'n' integer presentation type instead.
    
width
_____
*width* is a decimal integer defining the minimum field width. If not specified, then the field width will be determined by the content.
Preceding the width field by a zero ('0') character enables sign-aware zero-padding for numeric types. This is equivalent to a fill character of '0' with an alignment type of '='.

precision
_________
The precision is a decimal number indicating how many digits should be displayed after the decimal point for a floating point value formatted with 'f' and 'F', or before and after the decimal point for a floating point value formatted with 'g' or 'G'. For non-number types the field indicates the maximum field size - in other words, how many characters will be used from the field content. The precision is not allowed for integer values.

type
____
Determines how the data should be presented.

The available string presentation types are:

*'s'*
    String format. This is the default type for strings and may be omitted.
*None*
    The same as 's'.
    
The available integer presentation types are:

*'b'*
    Binary format. Outputs the number in base 2.
*'c'*
    Character. Converts the integer to the corresponding unicode character before printing.
*'d'*
    Decimal Integer. Outputs the number in base 10.
*'o'*
    Octal format. Outputs the number in base 8.
*'x'*
    Hex format. Outputs the number in base 16, using lower- case letters for the digits above 9.
*'X'*
    Hex format. Outputs the number in base 16, using upper- case letters for the digits above 9.
*'n'*
    Number. This is the same as 'd', except that it uses the current locale setting to insert the appropriate number separator characters.
*None*
    The same as 'd'.
    
In addition to the above presentation types, integers can be formatted with the floating point presentation types listed below (except 'n' and None). When doing so, float() is used to convert the integer to a floating point number before formatting.

The available presentation types for floating point and decimal values are:

*'e'*
    Exponent notation. Prints the number in scientific notation using the letter ‘e’ to indicate the exponent. The default precision is 6.
*'E'*
    Exponent notation. Same as 'e' except it uses an upper case ‘E’ as the separator character.
*'f'*
    Fixed point. Displays the number as a fixed-point number. The default precision is 6.
*'F'*
    Fixed point. Same as 'f'.
*'g'*
    General format. For a given precision p >= 1, this rounds the number to p significant digits and then formats the result in either fixed-point format or in scientific notation, depending on its magnitude.
    The precise rules are as follows: suppose that the result formatted with presentation type 'e' and precision p-1 would have exponent exp. Then if -4 <= exp < p, the number is formatted with presentation type 'f' and precision p-1-exp. Otherwise, the number is formatted with presentation type 'e' and precision p-1. In both cases insignificant trailing zeros are removed from the significand, and the decimal point is also removed if there are no remaining digits following it.
    Positive and negative infinity, positive and negative zero, and nans, are formatted as inf, -inf, 0, -0 and nan respectively, regardless of the precision.
    A precision of 0 is treated as equivalent to a precision of 1. The default precision is 6.
*'G'*
    General format. Same as 'g' except switches to 'E' if the number gets too large. The representations of infinity and NaN are uppercased, too.
*'n'*
    Number. This is the same as 'g', except that it uses the current locale setting to insert the appropriate number separator characters.
*'%'*
    Percentage. Multiplies the number by 100 and displays in fixed ('f') format, followed by a percent sign.
*None*
    The same as 'g'.
    
Return Value
------------
**str**

Time Complexity
---------------
#TODO

Remarks
-------
The string on which this method is called can contain literal text or replacement fields delimited by braces {}. Each replacement field contains either the numeric index of a positional argument, or the name of a keyword argument. Returns a copy of the string where each replacement field is replaced with the string value of the corresponding argument.

>>> "The sum of 1 + 2 is {0}".format(1+2)
'The sum of 1 + 2 is 3'

This method of string formatting is the new standard in Python 3, and should be preferred to the % formatting described in String Formatting Operations in new code.

Example 1
---------
>>> # accessing arguments by position:
>>> '{0}, {1}, {2}'.format('a', 'b', 'c')
'a, b, c'
>>> '{}, {}, {}'.format('a', 'b', 'c')  # 2.7+ only
'a, b, c'
>>> '{2}, {1}, {0}'.format('a', 'b', 'c')
'c, b, a'
>>> '{2}, {1}, {0}'.format(*'abc')      # unpacking argument sequence
'c, b, a'
>>> '{0}{1}{0}'.format('abra', 'cad')   # arguments' indices can be repeated
'abracadabra'

Example 2
---------
>>> # accessing arguments by name:
>>> 'Coordinates: {latitude}, {longitude}'.format(latitude='37.24N', longitude='-115.81W')
'Coordinates: 37.24N, -115.81W'
>>> coord = {'latitude': '37.24N', 'longitude': '-115.81W'}
>>> 'Coordinates: {latitude}, {longitude}'.format(**coord)
'Coordinates: 37.24N, -115.81W'

Example 3
---------
>>> # accessing arguments’ attributes:
>>> c = 3-5j
>>> ('The complex number {0} is formed from the real part {0.real} '
...  'and the imaginary part {0.imag}.').format(c)
'The complex number (3-5j) is formed from the real part 3.0 and the imaginary part -5.0.'
>>> class Point(object):
...     def __init__(self, x, y):
...         self.x, self.y = x, y
...     def __str__(self):
...         return 'Point({self.x}, {self.y})'.format(self=self)
...
>>> str(Point(4, 2))
'Point(4, 2)'

Example 4
---------
>>> # accessing arguments’ items:
>>> coord = (3, 5)
>>> 'X: {0[0]};  Y: {0[1]}'.format(coord)
'X: 3;  Y: 5'

Example 5
---------
>>> # replacing %s and %r:
>>> "repr() shows quotes: {!r}; str() doesn't: {!s}".format('test1', 'test2')
"repr() shows quotes: 'test1'; str() doesn't: test2"

Example 6
---------
>>> # aligning the text and specifying the width:
>>> '{:<30}'.format('left aligned')
'left aligned                  '
>>> '{:>30}'.format('right aligned')
'                 right aligned'
>>> '{:^30}'.format('centered')
'           centered           '
>>> '{:*^30}'.format('centered')  # use '*' as a fill char
'***********centered***********'

Example 7
---------
>>> # this example shows how to format numbers to specified precision
>>> "PI: {:.2f}".format(3.141592653589793)
'PI: 3.14'
>>> "PI: {:.2e}".format(3.141592653589793)
'PI: 3.14e+00'
>>> "PI: {:.2g}".format(3.141592653589793)
'PI: 3.1'
>>> "PI: {:.2n}".format(3.141592653589793)
'PI: 3.1'
>>> "PI: {:.2%}".format(3.141592653589793)
'PI: 314.16%'

Example 8
---------
>>> # replacing %+f, %-f, and % f and specifying a sign:
>>> '{:+f}; {:+f}'.format(3.14, -3.14)  # show it always
'+3.140000; -3.140000'
>>> '{: f}; {: f}'.format(3.14, -3.14)  # show a space for positive numbers
' 3.140000; -3.140000'
>>> '{:-f}; {:-f}'.format(3.14, -3.14)  # show only the minus -- same as '{:f}; {:f}'
'3.140000; -3.140000'

Example 9
---------
>>> # replacing %x and %o and converting the value to different bases:
>>> # format also supports binary numbers
>>> "int: {0:d};  hex: {0:x};  oct: {0:o};  bin: {0:b}".format(42)
'int: 42;  hex: 2a;  oct: 52;  bin: 101010'
>>> # with 0x, 0o, or 0b as prefix:
>>> "int: {0:d};  hex: {0:#x};  oct: {0:#o};  bin: {0:#b}".format(42)
'int: 42;  hex: 0x2a;  oct: 0o52;  bin: 0b101010'

Example 10
---------
>>> # using the comma as a thousands separator:
>>> '{:,}'.format(1234567890)
'1,234,567,890'

Example 11
----------
>>> # expressing a percentage:
>>> points = 19.5
>>> total = 22
>>> 'Correct answers: {:.2%}'.format(points/total)
'Correct answers: 88.64%'

Example 12
----------
>>> # using type-specific formatting:
>>> import datetime
>>> d = datetime.datetime(2010, 7, 4, 12, 15, 58)
>>> '{:%Y-%m-%d %H:%M:%S}'.format(d)
'2010-07-04 12:15:58'

Example 13
----------
>>> # nesting arguments and more complex examples
>>> for align, text in zip('<^>', ['left', 'center', 'right']):
...     '{0:{fill}{align}16}'.format(text, fill=align, align=align)
...
'left<<<<<<<<<<<<'
'^^^^^center^^^^^'
'>>>>>>>>>>>right'
>>>
>>> octets = [192, 168, 0, 1]
>>> '{:02X}{:02X}{:02X}{:02X}'.format(*octets)
'C0A80001'
>>> int(_, 16)
3232235521
>>>
>>> width = 5
>>> for num in range(5,12):
...     for base in 'dXob':
...         print '{0:{width}{base}}'.format(num, base=base, width=width),
...     print
...
    5     5     5   101
    6     6     6   110
    7     7     7   111
    8     8    10  1000
    9     9    11  1001
   10     A    12  1010
   11     B    13  1011

See Also
--------
#TODO
