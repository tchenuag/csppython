.. qnum::
   :start: 1
   :prefix: 01-10-

Conversion Functions
====================

**Learning Target: I can convert datatypes from one value to another.**

Any time we encounter code that generates an error, it's usually a good idea to find a way to make the code work without any errors.  So the big overarching question in this section is: **How do we combine different types?**

The Conversion Functions
------------------------

You would use **conversion functions** to *turn one datatype into another datatype.*

Table of the conversion functions:

	+-----------------------------------+-------------+
	| To convert to a String, use...    | ``str()``   |
	+-----------------------------------+-------------+
	| To convert to a Boolean, use...   | ``str()``   |
	+-----------------------------------+-------------+
	| To convert to a Float, use...     | ``float()`` |
	+-----------------------------------+-------------+
	| To convert to an Integer, use...  | ``int()``   |
	+-----------------------------------+-------------+

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

Checks for Understanding
------------------------

.. mchoice:: mc_convfunc_1
	:correct: b
	:answer_a: int
	:answer_b: float
	:answer_c: string
	:feedback_a: Which conversion function is being used?
	:feedback_b: Nice job!
	:feedback_c: Which conversion function is being used?

	What is the resulting datatype of the following expression? ``float("10")``

.. mchoice:: mc_convfunc_2
	:correct: c
	:answer_a: int
	:answer_b: float
	:answer_c: string
	:feedback_a: Which conversion function is being used?
	:feedback_b: Which conversion function is being used?
	:feedback_c: Nice job!

	What is the resulting datatype of the following expression? ``str(False)``

.. mchoice:: mc_convfunc_3
	:correct: c
	:answer_a: 2
	:answer_b: "2.3"
	:answer_c: 2.3
	:answer_d: "2"
	:feedback_a: What's the rule when the str() function is used?
	:feedback_b: Nice job!
	:feedback_c: What's the rule when the str() function is used?
	:feedback_d: What's the rule when the str() function is used?

	What is the result of the following expression? ``str(2.3)``

A Note on Errors
----------------

So what happens if you try to convert something like a word to an integer?  See for yourself:

.. activecode:: ac_convfunc_2
	:nocodelens:

	print int("ten")

Note the error.  Keep that in mind!  **Only strings that use digits can be converted to numbers.**

