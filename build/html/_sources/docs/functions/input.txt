=====
input
=====

Description
===========
Evaluates user input.

Syntax
======
**input** *([prompt])*

*prompt*
	Optional. The prompt text.

Return Value
============
#TODO

Time Complexity
============
#TODO

Note
====
Input is equivalent to eval(raw_input(prompt)).

Remarks
=======
This function does not catch user errors. If the input is not syntactically valid, a SyntaxError will be raised. Other exceptions may be raised if there is an error during evaluation.

If the readline module was loaded, then input() will use it to provide elaborate line editing and history features.
Consider using the raw_input() function for general input from users.

Example
=======
>>> input()
2+2
4
>>> input('Enter a valid python expression...\n')
Enter a valid python expression...
2*2
4

See Also
========
#TODO
