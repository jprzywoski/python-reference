=========
raw_input
=========

Description
===========
Reads a line from standard input stream.

Syntax
======
**raw_input** *([prompt])*

*prompt*
	Optional. Text that is displayed as a prompt.

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
If the prompt argument is present, it is written to standard output without a trailing newline. The function then reads a line from input, converts it to a string (stripping a trailing newline), and returns that. When EOF is read, EOFError is raised.
If the readline module was loaded, then raw_input() will use it to provide elaborate line editing and history features.

Example
=======
>>> s = raw_input()
hello
>>> s
'hello'
>>> s = raw_input('Please enter a value...')
Please enter a value...1000
>>> s
'1000'
>>> raw_input('Please enter a value...\n')
Please enter a value...
100
'100'

See Also
========
#TODO