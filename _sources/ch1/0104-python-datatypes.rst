.. qnum::
   :start: 1
   :prefix: 01-04-


Data Representation in Python
=============================

Lesson: What is data?
---------------------

Everything you see right now is data.  Cellular signals flying through the air is data.  A text message, a song, a video, is all data.  Even though data comes in many forms, there are some very *simple representations of data*, called **basic datatypes**, that we will be learning about.  

In Python, the five basic datatypes that we will be learning are:
	- ``int``

	  ``int`` is short for **integer**, which means any **whole number** (a number with no decimals).  In Python, a number is an int when it has no decimal point.  Integers are 32-bit, which mean they have a maximum value of 1 less than 2 to the power of ``32 (2^32 - 1)``, or ``4294967295``.

	  Examples of integers are: ``1, -402, 9999999``

	- ``float``

	  ``float`` is short for **floating point number**, which is a more specific way of representing numbers - this allows us to use decimals.  In Python, a number is a float when it has a decimal point and a number following the decimal point.  An float can represent an integer by adding .0 to the end of the number.

	  Examples of floats are: ``0.0001, -402.0, 1234.5678``

	- ``string``

	  A ``string`` is another way of saying **text** - representing letters, digits, and symbols.  In Python, data is a string when it is surrounded by single or double quotes.

	  Examples of strings are: ``"x", 'a string', "2#%a  bcd&  *1 *64jed#@ (*S )"``

	- ``boolean``

	  A ``boolean`` is a datatype with only two values - **True or False**.  In Python, boolean values are represented by the words ``True`` and ``False`` - no quotes - and be sure to capitalize the first letter!

	  The only two boolean values are: ``True, False``

	- ``NoneType``

	  The ``NoneType`` in python is a datatype that, interestingly enough, represents **no value**.  In Python, "no value" is represented by the word ``None`` - no quotes - and again, capitalize the first letter!

	  The only NoneType value is: ``None``

Practice: Check For Understanding
---------------------------------

.. mchoice:: question01_04_01
	:correct: c
	:answer_a: ``int``
	:answer_b: ``float``
	:answer_c: ``string``
	:answer_d: ``boolean``
	:feedback_a: int is short for integer, which is a number. Try again! Hint: What datatype uses quotes?
	:feedback_b: float is short for floating point number. Try again! Hint: What datatype uses quotes?
	:feedback_c: Great job - only strings will use quotes!
	:feedback_d: There are only two values for boolean - True and False. Try again! Hint: What datatype uses quotes?

	What datatype would ``"Nice to meet you!"`` be?

.. mchoice:: question01_04_02
	:multiple_answers:
	:correct: b,d
	:answer_a: ``boolean``
	:answer_b: ``int``
	:answer_c: ``string``
	:answer_d: ``float``
	:feedback_a: Boolean has two values, while there are certainly more than two numbers in existence!
	:feedback_b: integers are numbers!
	:feedback_c: Strings use quotes, which numbers don't need..
	:feedback_d: floats are short for floating point numbers!

	Which of the following datatypes represent types of numbers?

.. dragndrop:: question_01_04_03
	:feedback: You can look back to the notes if you need to!
	:match_1: float|||Decimal number
	:match_2: boolean|||True/False
	:match_3: int|||Whole number
	:match_4: NoneType|||Always None
	:match_5: string|||Text, uses quotes

	Drag the datatypes on the left to the description on the right.

.. dragndrop:: question_01_04_04
	:feedback: You can look back to the notes if you need to!
	:match_1: float|||5.0
	:match_2: boolean|||True
	:match_3: int|||10
	:match_4: NoneType|||None
	:match_5: string|||"5"

	Drag the datatypes on the left to the example on the right.