.. qnum::
   :start: 1
   :prefix: 01-11-

Introduction to Variables
=========================

**Learning Target: I can use variables to store Python data.**

Now that we know how to express data, we can save them away using **variables**.

Think of variables as a storage box with labels.  Variables have the following characteristics:
	- They can only hold one value at a time (although the value could be a list of values, which we will learn later)
	- They have a name which you can use to reference its held value (like the label on the box)
	- The name given to a variable cannot be changed
	- They can hold values of any type (not true for all programming languages)

There's two actions that we're going to learn:
	- Saving something into a variable
	- Getting something from a variable

Variable Creation / Storing into Variables
------------------------------------------

Let's start with how to name variables.  There are a few rules we have to follow when naming variables:
	- Variable names can only consist of uppercase letters, lowercase letters, digits, and underscores ( the character _ ).
	- Variable names cannot start with digits

.. mchoice:: cfu_var_1
	:multiple_answers:
	:correct: a,b,e
	:answer_a: NAME
	:answer_b: n4m3
	:answer_c: |\|4M3
	:answer_d: 1_name
	:answer_e: ______name_
	:feedback_a: Great job!
	:feedback_b: Great job!
	:feedback_c: Check the rules of what the name can contain!
	:feedback_d: What can variables not start with?
	:feedback_e: Great job!

	Select all valid variable names.

To store a value into a variable, you must use what's called a **variable assignment statement**.

Such a statement has three parts:
	- Left side: the name of the variable to store into
	- Equal sign in the middle
	- Right side: the value or expression to store into the variable name on the left

As an example, ``name = "Bob"`` would store the string ``"Bob"`` into a variable called ``name``.
The code ``name = "Leeroy" + "Jenkins"`` would store the string ``"LeeroyJenkins"`` into a variable called ``name``.  Note that the entire expression to the right of the equal sign is evaluated before getting saved into the variable.

Run the code below to observe the behavior of multiple assignment statements lining up.

.. activecode:: ac_var_1
	:nocodelens:

	num = 10
	print "\n\n" #this is to make the output line up, ignore this line
	print num
	num = 15
	print "\n\n" #same as before, ignore this line!
	print num

The four steps this code is executing are:
	- Set ``num`` to 10
	- Print the value of ``num`` (which is 10)
	- Set ``num`` to 15
	- Print the value of ``num`` (which is now 15)

Try the problem below to solidify your understanding.

.. parsonsprob:: cfu_var_1

	Order the code in the correct order that will correct set ``saying`` to ``"hello"``, then set ``saying`` to ``"goodbye"``, then print ``saying``.
	-----
	saying = "hello"
	saying = "goodbye"
	print saying

Retrieving From a Variable
--------------------------

To get a value from a variable, you just have to reference the variable name, either alone or as part of an expression.