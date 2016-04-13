.. qnum::
   :start: 1
   :prefix: 01-06-


Integer Division
================

**Learning Target: I can recognize when a quotient will give an less accurate result.**

If you experimented around with division and integers, you might have noticed something funny.  Run the code below as an example:

.. activecode:: ac_intdiv_1
	:nocodelens:
	:caption: Note that everything after the # is a comment and is not run as code

	print 1 / 2 #should be 0.5
	print 5 / 2 #should be 2.5
	print 8 / 3 #should be 2.3333

How Integer Division Works
--------------------------

**Integer Division** is when you divide an integer by another integer.  The result has to be an integer, so the decimal point and everything afterwards is cut off and removed.

Another way of saying it is when you divide an integer by another integer, the result is always *rounded down*, or taking the **"floor"** of the number.