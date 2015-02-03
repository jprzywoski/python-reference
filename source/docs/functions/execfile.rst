========
execfile
========

Description
===========
Evaluates contents of a file.

Syntax
======
**execfile** *(filename[, globals[, locals]])*

*filename*
	Required. A file to be parsed and evaluated as a sequence of Python statements (similarly to a module).
*globals*
	Optional. Any mapping object providing global namespace.
*locals*
	Optional. Any mapping object providing local namespace.

Return Value
============
#TODO

Time Complexity
============
#TODO

Remarks
=======
This function is similar to the exec statement, but parses a file instead of a string. It is different from the import statement in that it does not use the module administration — it reads the file unconditionally and does not create a new module.
Remember that at module level, globals and locals are the same dictionary. If two separate objects are passed as globals and locals, the code will be executed as if it were embedded in a class definition.

If the locals dictionary is omitted it defaults to the globals dictionary. If both dictionaries are omitted, the expression is executed in the environment where execfile() is called. The return value is None.

Note
====
The default locals act as described for function locals() below: modifications to the default locals dictionary should not be attempted. Pass an explicit locals dictionary if you need to see effects of the code on locals after function execfile() returns. execfile() cannot be used reliably to modify a function’s locals.

Example
=======
>>> execfile(r'C:\test.py') #test.py contains the following line: 'print "foo"'
foo

See Also
========
#TODO