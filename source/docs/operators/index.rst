=========
Operators
=========


Arithmetic Operators
====================
`+ (addition)`_
    Returns the sum of two expressions.
`- (subtraction)`_
    Returns the difference of two expressions.
`* (multiplication)`_
    Returns the product of two expressions.
`** (power)`_
    Returns the value of a numeric expression raised to a specified power.
`/ (division)`_
    Returns the quotient of two expressions.
`// (floor division)`_
    Returns the integral part of the quotient.
`% (modulus)`_
    Returns the decimal part (remainder) of the quotient.
    
Assignment Operators
====================
`= (simple assignment)`_
    Assigns a value to a variable(s).
`+= (increment assignment)`_
    Adds a value and the variable and assigns the result to that variable.
`-= (decrement assignment)`_
    Subtracts a value from the variable and assigns the result to that variable.
`*= (multiplication assignment)`_
    Multiplies the variable by a value and assigns the result to that variable.
`/= (division assignment)`_
    Divides the variable by a value and assigns the result to that variable.
`**= (power assignment)`_
    Raises the variable to a specified power and assigns the result to the variable.
`%= (modulus assignment)`_
    Computes the modulus of the variable and a value and assigns the result to that variable.
`//= (floor division assignment)`_
    Floor divides the variable by a value and assigns the result to that variable.

Relational Operators
====================
`== (equal)`_
    Returns a Boolean stating whether two expressions are equal.
`!= (not equal)`_
    Returns a Boolean stating whether two expressions are not equal.
`> (greater than)`_
    Returns a Boolean stating whether one expression is greater than the other.
`>= (greater than or equal)`_
    Returns a Boolean stating whether one expression is greater than or equal the other.
`< (less than)`_
    Returns a Boolean stating whether one expression is less than the other.
`<= (less than or equal)`_
    Returns a Boolean stating whether one expression is less than or equal the other.

Boolean Operators
=================
`and`_
    Returns the first operand that evaluates to *False* or the last one if all are *True*.
`or`_
    Returns the first operand that evaluates to *True* or the last one if all are *False*.
`not`_   
    Returns a boolean that is the reverse of the logical state of an expression.

Conditional Operator
====
`if else`_
    Returns either value depending on the result of a Boolean expression.
    
Identity
========
`is`_
    Returns a Boolean stating whether two objects are the same.
    
Membership
==========
`in`_
    Returns a Boolean stating whether the object is in the container.
    
Deletion
====
`del`_
    Removes object.

Callables Operators
==================
`* (tuple packing)`_
    Packs the consecutive function positional arguments into a tuple.
`** (dictionary packing)`_
    Packs the consecutive function keyword arguments into a dictionary.
`* (tuple unpacking)`_
    Unpacks the contents of a tuple into the function call.
`** (dictionary unpacking)`_
    Unpacks the contents of a dictionary into the function call.
`@ (decorator)`_
    Returns a callable wrapped by another callable.
`() (call operator)`_
    Calls a callable object with specified arguments.
`lambda`_
    Returns an anonymous function.

Bitwise Operators
=================
`& (bitwise AND)`_
    Returns the result of bitwise AND of two integers.
`| (bitwise OR)`_
    Returns the result of bitwise OR of two integers.
`^ (bitwise XOR)`_
    Returns the result of bitwise XOR of two integers.
`<< (left shift)`_
    Shifts the bits of the first operand left by the specified number of bits.
`>> (right shift)`_
    Shifts the bits of the first operand right by the specified number of bits.
`~ (bitwise complement)`_
    Sets the 1 bits to 0 and 1 to 0 and then adds 1.
    
Bitwise Assignment Operators
============================
`&= (bitwise AND assignment)`_
    Performs bitwise AND and assigns value to the left operand.
`|= (bitwise OR assignment)`_
    Performs bitwise OR and assigns value to the left operand.
`^= (bitwise XOR assignment)`_
    Performs bitwise XOR and assigns value to the left operand.
`<<= (bitwise right shift assignment)`_ 
    Performs bitwise left shift and assigns value to the left operand.
`>>= (bitwise left shift assignment)`_
    Performs bitwise right shift and assigns value to the left operand.

Misc
====
`; (statement separator)`_
    Separates two statements.
`\ (line continuation)`_
    Breaks the line of code allowing for the next line continuation.
`. (attribute access)`_
    Gives access to an object's attribute.

String and Sequence Operators
====
`+ (concatenation)`_
    Returns a concatenation of two sequences.
`* (multiple concatenation)`_
    Returns a sequence self-concatenated specified amount of times.
`% (string formatting operator)`_
    Formats the string according to the specified format.

Sequence Assignment Operators
====
`+= (concatenation assignment)`_
    Concatenates the sequence with the right operand and assigns the result to that sequence.
`*= (multiple concatenation assignment)`_
    Multiple concatenates the sequence and assigns the result to that sequence.
    
    
.. _is: is.html
.. _in: in.html
.. _+ (addition): addition.html
.. _- (subtraction): subtraction.html
.. _* (multiplication): multiplication.html
.. _** (power): exponent.html
.. _/ (division): division.html
.. _// (floor division): floor_division.html
.. _% (modulus): modulus.html
.. _and: and.html
.. _or: or.html
.. _not: not.html
.. _not: not.html
.. _= (simple assignment): assignment.html
.. _+= (increment assignment): addition_assignment.html
.. _-= (decrement assignment): subtraction_assignment.html
.. _*= (multiplication assignment): multiplication_assignment.html
.. _/= (division assignment): division_assignment.html
.. _**= (power assignment): exponent_assignment.html
.. _%= (modulus assignment): modulus_assignment.html
.. _//= (floor division assignment): floor_division_assignment.html
.. _== (equal): equal.html
.. _!= (not equal): not_equal.html
.. _> (greater than): greater_than.html
.. _>= (greater than or equal): greater_eq.html
.. _< (less than): less_than.html
.. _<= (less than or equal): less_eq.html
.. _if else: ternary.html
.. _* (tuple packing): tuple_pack.html
.. _** (dictionary packing): dict_pack.html
.. _* (tuple unpacking): tuple_unpack.html
.. _** (dictionary unpacking): dict_unpack.html
.. _@ (decorator): decorator.html
.. _() (call operator): call.html
.. _& (bitwise AND): bitwise_AND.html
.. _| (bitwise OR): bitwise_OR.html
.. _^ (bitwise XOR): bitwise_XOR.html
.. _<< (left shift): bitwise_left_shift.html
.. _>> (right shift): bitwise_right_shift.html
.. _~ (bitwise complement): bitwise_complement.html
.. _&= (bitwise AND assignment): bitwise_AND_assignment.html
.. _|= (bitwise OR assignment): bitwise_inclusive_OR_assignment.html
.. _^= (bitwise XOR assignment): bitwise_exclusive_OR_assignment.html
.. _>>= (bitwise left shift assignment): bitwise_left_shift_assignment.html
.. _<<= (bitwise right shift assignment): bitwise_right_shift_assignment.html
.. _; (statement separator): semicolon.html
.. _\ (line continuation): slash.html
.. _. (attribute access): attr_access.html
.. _+ (concatenation): concatenation.html
.. _* (multiple concatenation): multiple_concatenation.html
.. _% (string formatting operator): ../str/formatting.html
.. _+= (concatenation assignment): concatenation_assignment.html
.. _*= (multiple concatenation assignment): multiple_concatenation_assignment.html
.. _lambda: lambda.html

