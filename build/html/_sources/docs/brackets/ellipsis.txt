=====================
[ , ..., ] (ellipsis)
=====================

Description
===========
Gives access to a specified range of array's elements.

Syntax
======
**array** *[ , ..., ]*

Return Value
============
The same as selected.

Time Complexity
===============
#TODO

Remarks
=======

Ellipsis is used for slicing multidimensional numpy arrays.

The ellipsis syntax may be used to indicate selecting in full any remaining unspecified dimensions. 

Example
=======
::

    >>> n = numpy.arange(16).reshape(2, 2, 2, 2)
    >>> n
    array([[[[ 0,  1],
             [ 2,  3]],

            [[ 4,  5],
             [ 6,  7]]],


           [[[ 8,  9],
             [10, 11]],

            [[12, 13],
             [14, 15]]]])
    >>> n[1,...,1]            # equivalent to n[1,:,:,1]
    array([[ 9, 11],
           [13, 15]])
    >>> # also Ellipsis object can be used interchangeably
    >>> n[1, Ellipsis, 1]
    array([[ 9, 11],
           [13, 15]])
       
See Also
========
#TODO
