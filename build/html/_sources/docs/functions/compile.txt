=======
compile
=======

Description
===========
Returns an AST or code object.

Syntax
======
**compile** *(source, filename, mode[, flags[, dont_inherit]])*

*source*
	Required. source can either be a Unicode string, a Latin-1 encoded string or an AST object. Refer to the ast module documentation for information on how to work with AST objects.
*filename*
	Required. The filename argument should give the file from which the code was read; pass some recognizable value if it wasn’t read from a file ('<string>' is commonly used).
*mode*
	Required. The mode argument specifies what kind of code must be compiled;
    it can be 'exec' if source consists of a sequence of statements,
    'eval' if it consists of a single expression (note that you cannot use statements in this mode; only a (single) expression is valid),
    or 'single' if it consists of a single interactive statement (in the latter case, expression statements that evaluate to something other than None will be printed).
*flags, dont_inherit*
	Optional. The optional arguments flags and dont_inherit control which future statements (see PEP 236) affect the compilation of source. If neither is present (or both are zero) the code is compiled with those future statements that are in effect in the code that is calling compile. If the flags argument is given and dont_inherit is not (or is zero) then the future statements specified by the flags argument are used in addition to those that would be used anyway. If dont_inherit is a non-zero integer then the flags argument is it – the future statements in effect around the call to compile are ignored.
    
Future statements are specified by bits which can be bitwise ORed together to specify multiple statements. The bitfield required to specify a given feature can be found as the compiler_flag attribute on the _Feature instance in the __future__ module.

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
Though code objects represent some piece of executable code, they are not, by themselves, directly callable.
Code objects can be executed by an exec statement or evaluated by a call to eval().
This function raises SyntaxError if the compiled source is invalid and TypeError if the source contains null bytes.
See also exec statement,  eval() and execfile() functions.

Note
====
When compiling a string with multi-line code in 'single' or 'eval' mode, input must be terminated by at least one newline character. This is to facilitate detection of incomplete and complete statements in the code module.

Example 1
=========
>>> c = compile('2 + 2', '<string>', 'eval')
>>> print c
<code object <module> at 00CE7B60, file "", line 1>
>>> c.co_code
'd\x01\x00S'
>>> eval(c)
4

Example 2
=========
>>> code = compile('a = 1 + 2', '<string>', 'exec')
>>> exec code
>>> print a
3

Example 3
=========
>>> s = '''
... print "foo"
... print "bar"
... '''
>>> c = compile(s, '<string>', 'single')
>>> exec c
foo

Example 4
=========
>>> #This example executes code object against a new environment; that means the result won’t be injected into the global namespace
>>> code = compile('a = 1 + 2', '<string>', 'exec')
>>> ns = {}
>>> exec code in ns
>>> print ns['a']
3
>>> globals()['a']
Traceback (most recent call last):
  File "<interactive input>", line 1, in <module>
KeyError: 'a'

See Also
========
#TODO