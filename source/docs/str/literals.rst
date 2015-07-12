==============
Literal Syntax
==============

String literals can be enclosed in matching single quotes (') or double quotes (").

Example 1
=========
>>> 'ABC'
'ABC'
>>> "ABC"
'ABC'

String literal concatenation
----------------------------
Multiple adjacent string literals (delimited by whitespace), possibly using different quoting conventions, are allowed, and their meaning is the same as their concatenation. Thus, "hello" 'world' is equivalent to "helloworld". This feature can be used to reduce the number of backslashes needed, to split long strings conveniently across long lines, or even to add comments to parts of strings, for example:

::

    re.compile(
        "[A-Za-z_]"       # letter or underscore
        "[A-Za-z0-9_]*"   # letter, digit or underscore
    )

    
Note that this feature is defined at the syntactical level, but implemented at compile time. The ‘+’ operator must be used to concatenate string expressions at run time. Also note that literal concatenation can use different quoting styles for each component (even mixing raw strings and triple quoted strings).

Example 2
=========
>>> 'AB' "CD"
'ABCD'

Strings can be broken into two or more lines by using line continaution character:

Example 3
=========
>>> s = "AB\
... CD"
>>> s
'ABCD'

Unescaped quotes of the same type as the one that was used for creating the string can’t be used inside of it:

Example 4
=========
>>> "AB'CD"
"AB'CD"
>>> "AB"CD"
  File "<interactive input>", line 1
    "AB"CD"
           ^
SyntaxError: invalid syntax

Multi line strings
------------------
Strings can also be enclosed in matching groups of three single or double quotes (these are generally referred to as triple-quoted strings).

Example 5
=========
>>> '''AB
... CD
... '''
'AB\nCD\n'
>>> """AB
... CD
... """
'AB\nCD\n'

In triple-quoted strings, unescaped newlines and quotes are allowed (and are retained), except that three unescaped quotes in a row terminate the string. (A "quote" is the character used to open the string, i.e. either ' or ".)

Example 6
=========
>>> """
... AB "BC"
... """
'\nAB "BC"\n'
>>> '''
... AB 'BC'
... '''
"\nAB 'BC'\n"

The backslash (\\) character is used to escape characters that otherwise have a special meaning, such as newline, backslash itself, or the quote character.

Example 6
=========
>>> print "AA\nBB"
AA
BB
