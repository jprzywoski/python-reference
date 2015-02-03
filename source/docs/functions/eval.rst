====
eval
====

Description
===========
Returns a result of the evaluation of a Python expression.

Syntax
======
**eval** *(expression[, globals[, locals]])*

*expression*
	Required. The arguments are a Unicode or Latin-1 encoded string
*globals*
	Optional. A dictionary defining the namespace in which the expression is evaluated.
*locals*
	Optional. A dictionary defining the local namespace.

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
The expression argument is parsed and evaluated as a Python expression (technically speaking, a condition list) using the globals and locals dictionaries as global and local namespace. If the globals dictionary is present and lacks ‘__builtins__’, the current globals are copied into globals before expression is parsed. This means that expression normally has full access to the standard __builtin__ module and restricted environments are propagated. If the locals dictionary is omitted it defaults to the globals dictionary. If both dictionaries are omitted, the expression is executed in the environment where eval() is called. The return value is the result of the evaluated expression. Syntax errors are reported as exceptions.

This function can also be used to execute arbitrary code objects (such as those created by compile()). In this case pass a code object instead of a string. If the code object has been compiled with 'exec' as the mode argument, eval()‘s return value will be None.
Hints: dynamic execution of statements is supported by the exec statement. Execution of statements from a file is supported by the execfile() function. The globals() and locals() functions returns the current global and local dictionary, respectively, which may be useful to pass around for use by eval() or execfile().

See ast.literal_eval() for a function that can safely evaluate strings with expressions containing only literals.
See also exec statement and execfile() and compile() functions.

Example 1
=========
>>> x = 1
>>> print eval('x+1')
2
>>> eval('2*2')
4
>>> eval("len('bamf')")
4

Example 2
=========
>>> # this example shows how eval can access global namespace; this is a potential security hazard
>>> eval("os.getcwd()")
NameError: name 'os' is not defined
>>> import os
>>> eval("os.getcwd()")
'C:\\Program Files\\PyScripter'

Example 3
=========
>>> # this example shows how providing globals argument prevents eval from accessing real globals dictionary
>>> eval("os.getcwd()", {})
NameError: name 'os' is not defined
>>> # that example however can be bypassed by using __import__ function inside eval
>>> eval('__import__("os").getcwd()', {})
'C:\\Program Files\\PyScripter'

Example 4
=========
>>> # this example shows how to prevent eval from importing any modules
>>> eval('__import__("os").getcwd()', {'__builtins__': {}})
Traceback (most recent call last):
  File "<interactive input>", line 1, in <module>
  File "<string>", line 1, in <module>
NameError: name '__import__' is not defined

See Also
========
#TODO