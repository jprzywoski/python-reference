====
int
====

These represent numbers in the range -2147483648 through 2147483647. (The range may be larger on machines with a larger natural word size, but not smaller.) When the result of an operation would fall outside this range, the result is normally returned as a long integer (in some cases, the exception OverflowError is raised instead). For the purpose of shift and mask operations, integers are assumed to have a binary, 2’s complement notation using 32 or more bits, and hiding no bits from the user (i.e., all 4294967296 different bit patterns correspond to different values).

Plain integers (also just called integers) are implemented using long in C, which gives them at least 32 bits of precision (sys.maxint is always set to the maximum plain integer value for the current platform; the minimum value is -sys.maxint - 1). Long integers have unlimited precision.

Numbers are created by numeric literals or as the result of built-in functions and operators. Unadorned integer literals (including binary, hex, and octal numbers) yield plain integers unless the value they denote is too large to be represented as a plain integer, in which case they yield a long integer. Integer literals with an 'L' or 'l' suffix yield long integers ('L' is preferred because 1l looks too much like eleven!).

Constructors
====
`int()`_
    Returns an expression converted into an integer number.
`literal syntax`_
    Initializes a new instance of the **int** type.
    
Base Designators
====
`0... (Base Designators)`_
    Returns a decimal integer converted from the specified base.
    
Methods
====
`bit_length`_
    Returns the number of bits necessary to represent an integer in binary, excluding the sign and leading zeros.
    
.. _literal syntax: int_literals.html
.. _0... (Base Designators): base_designators.html
.. _bit_length: bit_length.html
.. _int(): ../functions/int.html
