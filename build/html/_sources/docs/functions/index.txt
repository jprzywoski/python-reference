==================
Built-In Functions
==================

Functional Programming
----------------------
`map`_
    Applies function to every item of an iterable object and returns a list of the results.
`filter`_
    Returns a sequence from those elements of iterable for which function returns true.
`reduce`_
    Applies function of two arguments cumulatively to the items of iterable, from left to right, so as to reduce the iterable to a single value.

Numeric Types Constructors
--------------------------
`bool`_
    Returns an expression that has been converted to a Boolean, using the standard truth testing procedure.
`int`_
    Converts a number or a string to an integer, or returns 0 if no arguments are given.
`long`_
    Converts a number or a string to a long integer, or returns 0 if no arguments are given.
`float`_
    Returns a floating point number.
`complex`_
    Returns a complex number.
    
Numeric Types Conversions
-------------------------
`bin`_
    Returns an expression that has been converted to a binary string.
`hex`_
    Converts an integer number (of any size) to a hexadecimal string.
`oct`_
    Converts an integer number to an octal string.
    
Arithmetic
----------
`abs`_
    Returns the absolute value of a number.
`pow`_
    Returns a number raised to a power; or optionally a modulus of the number raised to a power and another number.
`round`_
    Returns a floating point number rounded to a specified number of decimal places.
`divmod`_
    Returns quotient and remainder after a division of two numbers.
    
String Conversions
------------------
`chr`_
    Returns a string of one character whose ASCII code is the specified number.
`ord`_
    Returns an integer representing the code of the character.
`unichr`_
    Returns a Unicode character specified by the code.
`format`_
    Returns a formatted string.
`repr`_
    Returns a string containing a printable representation of an object.
    
Sequences Constructors
-----------------------
`str`_
    Returns a string containing a printable representation of an object.
`unicode`_
    Returns the Unicode string version of object.
`list`_
    Converts an object into a list.
`tuple`_
    Returns a tuple built from iterable.
`bytearray`_
    Returns a new array of bytes.
`buffer`_
    Returns a new buffer object which references the object argument.
`memoryview`_
    Returns a memoryview object.
`range`_
    Returns a list of arithmetic progressions.
`xrange`_
    Returns an xrange object.
    
Mappings Constructors
---------------------
`dict`_
    Returns a dictionary object.
`set`_
    Returns a set type initialized from iterable.
`frozenset`_
    Returns a frozenset object.
    
Operating on Containers
-----------------------
`enumerate`_
    Returns an enumerate object.
`len`_
    Returns an int type specifying number of elements in the collection.
`reversed`_
    Returns a reverse iterator over a sequence.
`sorted`_
    Returns a sorted list from the iterable.
`sum`_
    Returns a total of the items contained in the iterable object.
`zip`_
    Returns a list of tuples, where the i-th tuple contains the i-th element from each of the argument sequences or iterables.
`slice`_
    Returns a slice object.
    
Iterators
---------
`iter`_
    Returns an iterator object.
`next`_
    Retrieves the next item from the iterator by calling its next() method.
    
Comparisons
-----------
`cmp`_
    Compares two objects and returns an integer according to the outcome.
`max`_
    Returns the largest item in an iterable or the largest of two or more arguments.
`min`_
    Returns the smallest item from a collection.
`all`_
    Returns a Boolean value that indicates whether the collection contains only values that evaluate to True.
`any`_
    Returns a Boolean value that indicates whether the collection contains any values that evaluate to True.
Identity
--------
`hash`_
    Return the hash value of the object (if it has one).
`id`_
    Returns the “identity” of an object.
File Objects Constructors
-------------------------
`file`_
    Returns a file object.
`open`_
    Opens a file returning a file object.
Object Oriented Functions
-------------------------
`classmethod`_
    Returns a class method for the function.
`property`_
    Returns a property attribute for new-style classes (classes that derive from object).
`staticmethod`_
    Returns a static method for function.
`super`_
    Returns a proxy object that delegates method calls to a parent or sibling class of type.
`setattr`_
    Assigns a value to the object’s attribute given its name.
`getattr`_
    Returns the value of the named attribute of object.
`delattr`_
    Deletes the named attribute of an object.
`hasattr`_
    Returns a Boolean stating whether the object has the specified attribute.
`isinstance`_
    Returns a Boolean stating whether the object is an instance or subclass of another object.
`issubclass`_
    Returns a Bool type indicating whether an object is a subclass of a class.
`vars`_
    Returns the mapping of an object’s (writable) attributes.
`dir`_
    Returns the list of names in the current local scope. If supplied with an argument attempts to return a list of valid attributes for that object.
`type (1)`_
    Returns the type of an object (constructor name).
`type (2)`_
    Returns a new type object.
    
Information
-----------
`callable`_
    Returns a Boolean stating whether the object argument appears callable.
`globals`_
    Returns a dictionary representing the current global symbol table.
`locals`_
    Returns a dictionary representing the current local symbol table.
`help`_
    Invokes the built-in help system.
System
------
`__import__`_
    Imports a module.
`reload`_
    Reloads a previously imported module.
`compile`_
    Returns an AST or code object.
`execfile`_
    Evaluates contents of a file.
`eval`_
    Returns a result of the evaluation of a Python expression.
`input`_
    Evaluates user input.
`intern`_
    Enters the string into interned strings table (if not already there).
`print`_
    Returns a printed representation of the objects.
`raw_input`_
    Reads a line from standard input stream.
    
Misc
----
`object`_
    Returns a new featureless object.
`apply`_
    Returns the result of a function or class object called with supplied arguments.
`basestring`_
    This abstract type is the superclass for str and unicode. It cannot be called or instantiated, but it can be used to test whether an object is an instance of str or unicode.
`coerce`_
    Returns a tuple consisting of the two numeric arguments converted to a common type.

.. _map: ../functions/map.html
.. _filter: ../functions/filter.html
.. _reduce: ../functions/reduce.html
