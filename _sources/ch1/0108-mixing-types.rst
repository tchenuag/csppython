.. qnum::
   :start: 1
   :prefix: 01-06-


Mixing Datatypes
================

Now that we know that we can use operators to combine values, what happens if we combine values of different types?

Mixing Ints with Floats and Booleans
------------------------------------

When you mix integers, floats, and booleans together, interesting things happen.  There is a "hierarchy" of types in which combining a "greater" type and a "lesser" type will give you a result of the "greater" type.  The hierarchy is as follows:

``float`` > ``int`` > ``boolean``

To observe, run the following code:

.. activecode:: ac_mixtype_1
	:nocodelens:
	:caption: Note that everything after the # is a comment and is not run as code

	print 1 + 1		#int + int => int
	print 1.0 + 1.0	#float + float => float
	print 1 + 1.0 	#int + float => float
	print True + 1	#boolean + int => int
	print True + 1.0 #boolean + float => float

Types change as they are evaluated, piece by piece.  As an example, consider the expression ``1 + 2.0 - 

Mixing Strings with Anything
----------------------------

Conversion Functions
--------------------

