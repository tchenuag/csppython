.. qnum::
   :start: 1
   :prefix: 01-06-


Conversion Functions
====================

**Learning Target: I can convert datatypes from one value to another.**

Any time we encounter code that generates an error, it's usually a good idea to find a way to make the code work without any errors.  So the big overarching question in this section is: **How do we combine different types?**

The Conversion Functions
------------------------

You would use **conversion functions** to *turn one datatype into another datatype.*

Table of the conversion functions:

	+-----------------------------------+------------+
	| To convert to a String, use...    | str()      |
	+-----------------------------------+------------+
	| To convert to a Boolean, use...   | str()      |
	+-----------------------------------+------------+
	| To convert to a Float, use...     | float()    |
	+-----------------------------------+------------+
	| To convert to an Integer, use...  | int()      |
	+-----------------------------------+------------+

You would use these functions by putting the value you want to convert between the parentheses.  Try running the example below:

.. activecode:: ac_convfunc_1
	:nocodelens:

	print str(5.0) # float to string
	print str(1) # int to string
	print str(True) # boolean to string
	print int("5") # string to int
	print int(2.7) # float to int (lose decimals)
	print float("6.3") # string to float
	print float(3) # int to float
	print bool(1) # int to boolean
	print bool("True") # string to boolean

Here are a few notes for specific type to type conversions:

	+--------+--------+--------------------------------------------+
	| From   | To     | Note                                       |
	+========+========+============================================+
	| any    | string | put quotes around int                      |
	+--------+--------+--------------------------------------------+
	| int    | float  | put a .0 at the end                        |
	+--------+--------+--------------------------------------------+
	| float  | int    | drop everything after decimal point        |
	+--------+--------+--------------------------------------------+
	| string | int    | becomes an int if it looks like a number   |
	+--------+--------+--------------------------------------------+
	| string | float  | becomes a float if it looks like a number  |
	+--------+--------+--------------------------------------------+





