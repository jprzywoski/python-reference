=================
Escape Characters
=================

The recognized escape sequences are:

``\newline``
    Ignored	 
``\``
    Backslash (\\)
``\'``
    Single quote (')	 
``\"``
    Double quote (")	 
``\a``
    ASCII Bell (BEL)	 
``\b``
    ASCII Backspace (BS)	 
``\f``
    ASCII Formfeed (FF)	 
``\n``
    ASCII Linefeed (LF)	 
``\N{name}``
    Character named NAME in the Unicode database (Unicode only)	 
``\r``
    ASCII Carriage Return (CR)	 
``\t``
    ASCII Horizontal Tab (TAB)	 
``\uxxxx``
    Character with 16-bit hex value XXXX (Unicode only)	(1)
``\Uxxxxxxxx``
    Character with 32-bit hex value XXXXXXXX (Unicode only)	(2)
``\v``
    ASCII Vertical Tab (VT)	 
``\ooo``
    Character with octal value OOO	(3,5)
``\xhh``
    Character with hex value HH	(4,5)

Notes
=====
1.	Individual code units which form parts of a surrogate pair can be encoded using this escape sequence.

2.	Any Unicode character can be encoded this way, but characters outside the Basic Multilingual Plane (BMP) will be encoded using a surrogate pair if Python is compiled to use 16-bit code units (the default).

3.	As in Standard C, up to three octal digits are accepted.

4.	Unlike in Standard C, exactly two hex digits are required.

5.	In a string literal, hexadecimal and octal escapes denote the byte with the given value; it is not necessary that the byte encodes a character in the source character set. In a Unicode literal, these escapes denote a Unicode character with the given value.

Remarks
=======
Unless an 'r' or 'R' prefix is present, escape sequences in strings are interpreted according to rules similar to those used by Standard C. 
Unlike Standard C, all unrecognized escape sequences are left in the string unchanged, i.e., the backslash is left in the string. (This behavior is useful when debugging: if an escape sequence is mistyped, the resulting output is more easily recognized as broken.) It is also important to note that the escape sequences marked as “(Unicode only)” in the table above fall into the category of unrecognized escapes for non-Unicode string literals.

When an 'r' or 'R' prefix is present, a character following a backslash is included in the string without change, and all backslashes are left in the string. For example, the string literal r"\n" consists of two characters: a backslash and a lowercase 'n'. String quotes can be escaped with a backslash, but the backslash remains in the string; for example, r"\"" is a valid string literal consisting of two characters: a backslash and a double quote; r"\" is not a valid string literal (even a raw string cannot end in an odd number of backslashes). Specifically, a raw string cannot end in a single backslash (since the backslash would escape the following quote character). Note also that a single backslash followed by a newline is interpreted as those two characters as part of the string, NOT as a line continuation.

When an 'r' or 'R' prefix is used in conjunction with a 'u' or 'U' prefix, then the \uXXXX and \UXXXXXXXX escape sequences are processed while all other backslashes are left in the string. For example, the string literal ur"\u0062\n" consists of three Unicode characters: ‘LATIN SMALL LETTER B’, ‘REVERSE SOLIDUS’, and ‘LATIN SMALL LETTER N’. Backslashes can be escaped with a preceding backslash; however, both remain in the string. As a result, \uXXXX escape sequences are only recognized when there are an odd number of backslashes.

Additionally, you can express any character by its numerical ASCII code by writing a backslash character \\ followed by the ASCII code expressed as an octal (base-8) or hexadecimal (base-16) number. In the first case (octal) the digits must immediately follow the backslash (for example \23 or \40), in the second case (hexadecimal), an x character must be written before the digits themselves (for example \x20 or \x4A).

Example 1
=========
>>> # this example writes a string "ABC" using hex
>>> "\x41\x42\x43"
'ABC'

Example 2
=========
>>> # this time using octal
>>> "\101\102\103"
'ABC'

