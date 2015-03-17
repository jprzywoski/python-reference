==========
__import__
==========

Description
===========
Imports a module.

Syntax
======
**__import__** *(name[, globals[, locals[, fromlist[, level]]]])*

*name*
	Required. Name of the module to import.
*globals*
	Optional. Dictionary of global names used to determine how to interpret the name in a package context.
*locals*
	Optional. Dictionary of local names names used to determine how to interpret the name in a package context. The standard implementation does not use its locals argument at all, and uses its globals only to determine the package context of the import statement.
*fromlist*
	Optional. The fromlist gives the names of objects or submodules that should be imported from the module given by name.
*level*
	Optional. level specifies whether to use absolute or relative imports. The default is -1 which indicates both absolute and relative imports will be attempted. 0 means only perform absolute imports. Positive values for level indicate the number of parent directories to search relative to the directory of the module calling __import__().

Return Value
============
#TODO

Time Complexity
============
#TODO

Note
====
This is an advanced function that is not needed in everyday Python programming, unlike importlib.import_module().

Remarks
=======
This function is invoked by the import statement. It can be replaced (by importing the __builtin__ module and assigning to __builtin__.__import__) in order to change semantics of the import statement, but nowadays it is usually simpler to use import hooks (see PEP 302). Direct use of __import__() is rare, except in cases where you want to import a module whose name is only known at runtime.

When the name variable is of the form package.module, normally, the top-level package (the name up till the first dot) is returned, not the module named by name. However, when a non-empty fromlist argument is given, the module named by name is returned.
For example, the statement import spam results in bytecode resembling the following code:

>>> spam = __import__('spam', globals(), locals(), [], -1)

The statement import spam.ham results in this call:

>>> spam = __import__('spam.ham', globals(), locals(), [], -1)

Note how __import__() returns the toplevel module here because this is the object that is bound to a name by the import statement.

On the other hand, the statement `from spam.ham import eggs, sausage as saus` results in

>>> _temp = __import__('spam.ham', globals(), locals(), ['eggs', 'sausage'], -1)
>>> eggs = _temp.eggs
>>> saus = _temp.sausage

Here, the spam.ham module is returned from __import__(). From this object, the names to import are retrieved and assigned to their respective names.

If you simply want to import a module (potentially within a package) by name, use importlib.import_module().

Example
====
#TODO

See Also
========
#TODO