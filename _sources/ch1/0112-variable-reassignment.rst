.. qnum::
   :start: 1
   :prefix: 01-12-

Variable Reassignment
=====================

**Learning Target: I can use alter a variable's value in a relative manner.**

With lots of experience in math and little experience in programming, when you see something like this:

``x = x + 1``

Red flags should instantly go off in your head.  How can ``x`` be equal to itself plus 1??  Can ``5`` be equal to ``6``?  No, of course not!

What you should not forget, however, is that the ``=`` symbol in programming is different from the ``=`` symbol in mathematics.

To review, the equal sign means **variable assignment** - it has a very specific purpose.

Recall the meaning of the left and right side of a variable assignment statement:
	- Left side: the variable to store into
	- Right side: the value **or expression** to store

An important thing to note is that the right side is always evaluated **before** being saved into the variable on the left.  This gives the line of code ``x = x + 1`` a whole new meaning.  Let's break it down:

Given a statement ``x = x + 1``, let's assume the value of ``x`` is currently ``0``.  Since it is an assignment statement, the right side of the equal sign, or ``x + 1``, gets evaluated first.  Since ``x`` is a variable being used in an expression, we use its actual value instead, which is ``0``.  So the expression being evaluated is ``0 + 1``, which is just ``1``.  This leaves us with the statement ``x = 1``, which then allows us to store ``1`` in ``x``, effectively increasing the value of ``x`` by ``1``.

However, this would have worked with any value of ``x``!  Let's say ``x`` was ``28``.  The expression ``x + 1`` would then be ``28 + 1``, or ``29``, which then gets saved back into ``x``.  ``x`` is effectively changed from ``28`` to ``29``, which is the same thing as increasing it by ``1``.

Let's run through some example code below, step by step.

.. codelens:: cl_reassign_1

	num = 10
	num = num + 5
	num = num * 2
	print num