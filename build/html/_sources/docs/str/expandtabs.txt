==========
expandtabs
==========

Description
----------
Returns a copy of the string where all tab characters were replaced by spaces.

Syntax
------
**str**. *expandtabs([tabsize])*

*tabsize*
    Optional. Size of the tab; default step is 8.

Return Value
------------
**str**

Time Complexity
---------------
#TODO

Remarks
-------
Tab positions occur every *tabsize* characters (default is 8, giving tab positions at columns 0, 8, 16 and so on). To expand the string, the current column is set to zero and the string is examined character by character. If the character is a tab (\t), one or more space characters are inserted in the result until the current column is equal to the next tab position. (The tab character itself is not copied.) If the character is a newline (\n) or return (\r), it is copied and the current column is reset to zero. Any other character is copied unchanged and the current column is incremented by one regardless of how the character is represented when printed.

Example
-------
>>> "AA\tBB\n".expandtabs()
'AA      BB\n'
>>> "AA\tBB\n".expandtabs(4)
'AA  BB\n'

See Also
--------
#TODO