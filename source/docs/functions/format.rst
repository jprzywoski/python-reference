======
format
======

Description
===========
Returns a formatted string.

Syntax
======
**format** *(value[, format_spec])*

*value*
	Optional.  A type to be formatted.
*format_spec*
	Optional.  If omitted returns a string representation of an object. General form:
    
**[[fill]align][sign][#][0][width][,][.precision][type]**

See below for details.

Fill
====
If a valid align value is specified, it can be preceded by a fill character that can be any character and defaults to a space if omitted.

Align
======
*'<'*
	Forces the field to be left-aligned within the available space (this is the default for most objects).
*'>'*
	Forces the field to be right-aligned within the available space (this is the default for numbers).
*'='*
	Forces the padding to be placed after the sign (if any) but before the digits. This is used for printing fields in the form ‘+000000120’. This alignment option is only valid for numeric types.
*'^'*
	Forces the field to be centered within the available space.
    
Sign
====
*'+'*
	indicates that a sign should be used for both positive as well as negative numbers.
*'-'*
	indicates that a sign should be used only for negative numbers (this is the default behavior).
*‘ ‘ (space)*
	indicates that a leading space should be used on positive numbers, and a minus sign on negative numbers.
*‘#’*
    The '#' option is only valid for integers, and only for binary, octal, or hexadecimal output. If present, it specifies that the output will be prefixed by '0b', '0o', or '0x', respectively.
*‘,’*
    The ',' option signals the use of a comma for a thousands separator. For a locale aware separator, use the 'n' integer presentation type instead.
    
Width
=====
*width* is a decimal integer defining the minimum field width. If not specified, then the field width will be determined by the content.
Preceding the width field by a zero ('0') character enables sign-aware zero-padding for numeric types. This is equivalent to a fill character of '0' with an alignment type of '='.

Precision
=========
The precision is a decimal number indicating how many digits should be displayed after the decimal point for a floating point value formatted with 'f' and 'F', or before and after the decimal point for a floating point value formatted with 'g' or 'G'. For non-number types the field indicates the maximum field size - in other words, how many characters will be used from the field content. The precision is not allowed for integer values.

Type
====
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
============
#TODO

Time Complexity
============
#TODO

Note
====
*format(value, format_spec)* merely calls *value.__format__(format_spec)*.

Example 1
=========
>>> #This example illustrates the use of [fill]align][width] options
>>> format(3.14, '0>10')
'0000003.14'
>>> format(3.14, '0>5')
'03.14'
>>> format(3.14, '#>5')
'#3.14'
>>> format(3.14, '#>10')
'######3.14'
>>> format(7, '#^10')
'####7#####'

Example 2
=========
>>> #This example illustrates the use of [sign] option
>>> format(7, '-')
'7'
>>> format(-7, '+')
'-7'
>>> format(-7, ' ')
'-7'
>>> format(7, ' ')
' 7'

Example 3
=========
>>> #This example illustrates the use of [#] option
>>> format(10, '0b')
'1010'
>>> format(10, '0o')
'12'
>>> format(10, '0x')
'a'

Example 4
=========
>>> #This example illustrates the use of [,] option
>>> format(16777216, ',')
'16,777,216'
>>> format(16777216, 'n')
'16777216'

Example 5
=========
>>> #This example illustrates the use of [precision] option
>>> format(16.777, '.1f')
'16.8'
>>> format(16.777, '.2f')
'16.78'
>>> format(16.777, '.3f')
'16.777'
>>> format(16.777, '.7f')
'16.7770000'

Example 6
=========
>>> #This example illustrates the use of [type] option on integers
>>> format(2, 'b')
'10'
>>> format(2, 'b')
'10'
>>> format(2, 'c')
'\x02'
>>> format(2, 'd')
'2'
>>> format(100, 'o')
'144'
>>> format(100, 'x')
'64'
>>> format(100, 'n')
'100'
>>> format(100)
'100'

Example 7
=========
>>> #This example illustrates the use of [type] option on floats
>>> format(3.13592, 'e')
'3.135920e+00'
>>> format(3.13592, 'E')
'3.135920E+00'
>>> format(3.13592, 'f')
'3.135920'
>>> format(3.13592, 'g')
'3.13592'
>>> format(3.13592, '.2g')
'3.1'
>>> format(3.13592, '%')
'313.592000%'
>>> format(3.13592, '.2%')
'313.59%'
>>> format(3.13592, 'n')
'3.13592'

See Also
========
#TODO
