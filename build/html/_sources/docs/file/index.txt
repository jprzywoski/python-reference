=====
file
=====

`Overview`_

Constructors
------------
`file()`_

Methods
-------
`flush`_
    Flushes the write buffers of the file.
`close`_
    Flushes and closes the file.
`fileno`_
    Returns the integer "file descriptor".
`next`_
    Returns a next line from the file.
`isatty`_
    Returns True if the file is if the stream is interactive (i.e., connected to a terminal/tty device).
`xreadlines`_
    Returns an iterator over the lines of the file.
`read`_
    Returns specified amount of bytes from the file.
`readline`_
    Reads one entire line from the file.
`readlines`_
    Returns a list containing lines from the file.
`seek`_
    Sets the file’s current position.
`tell`_
    Returns the file’s current position.
`truncate`_
    Truncates the file’s size.
`write`_
    Writes a string to the file.
`writelines`_
    Writes a sequence of strings to the file.

Properties
----------
`closed`_
    Returns a Boolean stating whether the file is closed.
`encoding`_
    Returns the encoding that this file uses.
`errors`_
    Returns the Unicode error handler used along with the encoding.
`mode`_
    Returns the I/O mode for the file.
`name`_
    Returns the name of the file.
`newlines`_
    Return type of newlines encountered while reading the file.
`softspace`_
    Returns a Boolean that indicates whether a space character needs to be printed before another value when using the print statement.
    
.. _Overview: overview.html
.. _flush: flush.html
.. _close: close.html
.. _fileno: fileno.html
.. _next: next.html
.. _isatty: isatty.html
.. _xreadlines: xreadlines.html
.. _read: read.html
.. _readline: readline.html
.. _readlines: readlines.html
.. _seek: seek.html
.. _tell: tell.html
.. _truncate: truncate.html
.. _write: write.html
.. _writelines: writelines.html
.. _closed: closed.html
.. _encoding: encoding.html
.. _errors: errors.html
.. _mode: mode.html
.. _name: name.html
.. _newlines: newlines.html
.. _softspace: softspace.html
