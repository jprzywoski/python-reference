====
code
====
Code objects represent byte-compiled executable Python code, or bytecode. The difference between a code object and a function object is that the function object contains an explicit reference to the function’s globals (the module in which it was defined), while a code object contains no context; also the default argument values are stored in the function object, not in the code object (because they represent values calculated at run-time). Unlike function objects, code objects are immutable and contain no references (directly or indirectly) to mutable objects.

Methods
=======
`co_argcount`_
    
`co_cellvars`_

`co_code`_

`co_consts`_

`co_filename`_

`co_firstlineno`_

`co_flags`_

`co_freevars`_

`co_lnotab`_

`co_name`_

`co_names`_

`co_nlocals`_

`co_stacksize`_

`co_varnames`_


.. _co_argcount: argcount.html
.. _co_cellvars: cellvars.html
.. _co_code: code.html
.. _co_consts: consts.html
.. _co_filename: filename.html
.. _co_firstlineno: firstlineno.html
.. _co_flags: flags.html
.. _co_freevars: freevars.html
.. _co_lnotab: lnotab.html
.. _co_name: name.html
.. _co_names: names.html
.. _co_nlocals: nlocals.html
.. _co_stacksize: stacksize.html
.. _co_varnames: varnames.html

