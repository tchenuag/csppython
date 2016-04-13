.. qnum::
   :start: 1
   :prefix: 01-07-

Operators and Booleans
======================

**Learning Target: I can use booleans in mathematical expressions.**

A Simple Explanation
--------------------

Remember that Booleans represent two values, ``True`` and ``False``.  But each of these also have integer values, as well!

	+---------------+-----------+
	| Boolean Value | Int Value |
	+===============+===========+
	| True          | 1         |
	+---------------+-----------+
	| False	        | 0         |
	+---------------+-----------+

Whenever you run code that uses any of the PEMDAS operators on True or False, it will just use their integer values.

Example:

.. activecode:: ac_bool_1
	:nocodelens:

	print True + True # 1+1
	print True + False # 1+0
	print False + False # 0+0
	print False - True # 0-1
	print True
	print False

Note that the boolean will only be used as an integer when combined with an operator!