============
Introduction
============

This documentation is the result of my frustration with official Python Manuals.

Currently all the material resides on my PC in a form of Word documents. I am going to convert those word documents into .rst files over the course of the next few days. Or weeks possibly if my motivation falters. And I'm talking about 300-400 A4 pages describing all the Python features with working code examples. It took me about 4 months to put it all together.

*Note*

Moving stuff from Word files into reStructuredText is tedious. This is work in progress as of January 2015.


*Update 18/01/2015.*

Moving all the contents from word files to Sphinx project has proven to be more time consuming than I originally thought. Getting the ver. 1.0 ready will take weeks.

Scope
=====

Everything here is intended for Python 2.7.X. The reason is simple - this is the version I personally use and its specification is frozen (no new features will be added), so the content is bound to be up to date for good. Moreover, Python 3.X is not catching up - there's like seven or eight people using it worldwide.

This work is not meant to be a total replacement for Python Manuals. As a matter of fact most of the definitions here are based on the official docs. I decided to only cover the core Python's syntax, that means, the stuff that does not require using "import" statement.

This reference is designed to minimize the amount of time needed to look things up. The whole layout is well structured and consistent. I put a lot of emphasis on working code examples and very simple definitions. Being realistic, no one wants to read lengthy passages about some obscure functions, most people only need to glance at the code examples and then copy, paste and modify.

Python Standard Library is beyond the scope of this reference. If you are looking for a description of library modules have a look at:

* Python Module of The Week by Doug Hellman

* Python Reference by Frederik Lundh (this one is a bit dated, but still top-notch in terms of clarity)

* Official Python Standard Library documentation (terse and lacks examples)


Rationale
=========

Python is such a well-designed, clean and enjoyable to code in language so it sure deserves to have a decent syntax reference. I’ve been coding in Python for a few months now and whenever I need to check something about syntax 99.9% of the time I end up either on Stackoverflow or some other on-line resource. My main gripes with official docs are too terse descriptions and virtual lack of any code examples as well as lack of any coherent logical structure. It does not have to be this way. Just take a look on Mozilla’s JavaScript reference or Microsoft’s any .net language or VBA/VBScript references. Those are excellent examples of good technical writing.

Absurdly enough the whole Python documentation stands in contrast to the Zen of Python.

My first idea was to identify main use case scenarios for using any language reference. Luckily there are only two I can think of:

#. I know what I am looking for and I only need a quick refresher on syntax or code snippet to copy/paste end edit for my needs.

#. I want to see if what I need to do has already been implemented (good example is **enum()** function – lots of people implement that pattern themselves). In this case I need to be quickly able to scan through a list of descriptions gathered in one place.

In both cases Python docs fail miserably.

So I decided to introduce the following template logical structures:

Use case 1
----------

This one is used to explain usage of functions/methods. It quickly gives you the info about:

* what does the function do

* what are the inputs

* what is the output

--------------------------------------------------------------------------------

Name
----

[quick description field – preferably up to 80 characters long]

Syntax
______

[detailed description of calling this function]

Return Value
____________

[if applicable]

Time Complexity
_______________

[if applicable]

Remarks
_______

[further discussion]

Examples
________

[simple code snippets to illustrate basic usage; the simpler the better]

See Also
________

[links to related topics]

Use case 2
----------

Used as a list of thematically grouped functions/methods. I decided to organize things by function rather than alphabetically. That's the same way a handyman organizes his tools in the toolbox. Makes needed things easier to find.

--------------------------------------------------------------------------------

Group
-----

**Method_a (hyperlink)**

   [quick description field – preferably up to 80 characters long]
   
**Method_b (hyperlink)**

   [quick description field – preferably up to 80 characters long]
   
