====
float
====

These represent machine-level double precision floating point numbers. You are at the mercy of the underlying machine architecture (and C or Java implementation) for the accepted range and handling of overflow. Python does not support single-precision floating point numbers; the savings in processor and memory usage that are usually the reason for using these is dwarfed by the overhead of using objects in Python, so there is no reason to complicate the language with two kinds of floating point numbers.

Floating point numbers are usually implemented using double in C; information about the precision and internal representation of floating point numbers for the machine on which your program is running is available in sys.float_info.

Constructors
====
`float()`_
    Returns an expression converted into a floating point number.
`literal syntax`_
    Initializes a new instance of the **float** type.

Scientific Notation
====
`e | E (scientific notation)`_
    Returns a float multiplied by the specified power of 10.

Methods
====
`as_integer_ratio`_
    Returns a pair of integers whose ratio is exactly equal to the original float and with a positive denominator.
`is_integer`_
    Returns True if the float instance is finite with integral value, and False otherwise.
`hex`_
    Returns a representation of a floating-point number as a hexadecimal string.
`fromhex`_
    Returns the float represented by a hexadecimal string s.
    

.. _literal syntax: ../float/literals.html
.. _as_integer_ratio: ../float/as_integer_ratio.html
.. _is_integer: ../float/is_integer.html
.. _hex: ../float/hex.html
.. _fromhex: ../float/fromhex.html
.. _e | E (scientific notation): ../float/scientific.html
.. _float(): ../functions/float.html
