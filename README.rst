python_learners_glossary
========================

Definitions of Pardon jargon to help Python beginners understand Pythonista gobbletigook

Basic
-----

.. _execute:

Execute
  Go.  Run.  Do that thing you do.  Nothing to do
  with beheading anybody.

Data
----

.. _value:

Value
  A single piece of data, like ``3`` or ``'Fluffy'``

String
  A piece of text data, like ``'hello'``.  Enclosing it
  in quotation marks
  tells Python that it's a string and not something like
  a variable name.

Float
  Short for *floating-point number*, a number with a
  decimal point.

.. _variable:

Variable
  A piece of data that has a name.

  ::

      cat_name = 'Fluffy'

  Now ``cat_name`` is a *variable* with the value 'Fluffy'.

Assign
  Give a name to a value_, making a variable_.

Dunder
  The two underscores before and after a method name to indicate that it is "magic", i.e. __init__, __new__, etc.

Magic Method
  Methods that can be used to change the normal behavior of an object. HINT : in Python, everything is an object.

Object
  A logical grouping of methods, expressions, variables, and functions.

Expression
  In Python, this is basically a list of commands that need to be evaluated and executed. Typically, these fit on one line, but there is a way for an expression to take up more than one line.

.. _list:

List
  A series of values.  Python will remember what order they
  come in.

  ::

      ['Mouser', 17, 'Whiskers']

<<<<<<< HEAD
Tuple
  A series of values.  Python will remember what order they
  come in.

  Hey, is that the same as a list_?  It's very similar, but
  after a tuple is set up, you're not allowed to change
  it.

  ::

      ('Mouser', 17, 'Whiskers')

Set
  Just like in mathematics - a group of values.  Python
  will *not* necessarily remember what order they came
  in, and each value_ can only appear in the set once.

Functions
---------

.. _function:

Function
  A named series of instructions.  Its definition
  begins with the `def` keyword.

  ::

      def feed_cat(kg_of_food, kg_of_cat):
          kg_of_food = kg_of_food - 0.1
          kg_of_cat = kg_of_cat + 0.1

.. _call:
.. _called:

Call
  Tell a function_ to execute_.  To call a
  function, give its name followed by
  parenthesis containing its arguments_ (if
  any).

  ::

      feed_cat(8.0, 3.0)

.. _argument:
.. _arguments:

Argument
  A piece of data that you "pass" (give) to a
  function_ as you call_ it.  In our ``feed_cat``
  function_, ``kg_of_food`` and ``kg_of_cat`` are
  the function's arguments.

Parameter
  Synonym for argument_.

Return
  Stop running a function_ and return to the place
  where the function was called_ from.  Send a
  value_ back - the "return value".

Object-oriented
---------------

.. _object:
.. _objects:

Object
  Contains both data and methods_.

Method
  A function that *belongs to* an object and
  "knows" about the object it belongs to.
  For instance, if `my_cat` is an object
  that has a `speak` method, then we can
  call_ it::

      my_cat.speak()
      'meow'

  ... and `my_cat.speak` doesn't need to be told what
  kind of animal should speak, because it already
  knows that it belongs to `my_cat`.

.. attribute_:

Attribute
  A piece of data that belongs to an object.

.. _class:
.. _classes:

Class
  TODO

Instance
  An object_ of a given class_.  `my_cat` is an
  *instance* of the class `Cat`.

Instantiate
  Create a new `instance` of a given class.
  When `my_cat` has kittens, she is instantiating
  several new instances of the class `Cat`.
  (Please spay our neuter your pets!)

Object-oriented programming
  Programming that makes use of classes_ and objects_.

Program Structure
-----------------

.. _module:

Module
  A single file of Python commands.  Calling it a
  module implies we plan to "import" it, not just
  call it on its own.

.. _package:

Package
  A directory full of modules that can all together
  be referred to by the package's name.

Import
  Make the contents of a module_ or package_ available
  in your current program, even though it comes outside
  your current program's file.

Tools
-----

.. _editor:

Editor
  A program to create or change files.  We usually mean
  *text editor*, since a Python program is a kind of
  text file.  Notepad is an example of an editor
  (but don't use Notepad to edit Python, it can
  introduce mistakes into your Python programs;
  `Notepad++`_ is a good alternative).

.. _`Notepad++`: https://notepad-plus-plus.org/

IDE
  Abbreviation for Integrated Development Environment.
  A kind of text editor_ with programming-related
  superpowers; a program that lets you build more programs.
  Examples include Eclipse, Sublime, Wingware, and IDLE


.. git_:

Git
  A program for `vesion control`_.

Mercurial
  A `version control`_ tool.  It's less popular than
  git_, even though it's written in pure Python,
  but accomplishes basically the same things.

Database
  A place to store data outside the program,
  possibly in memory ("in-memory databases")
  but generally on disk.  A file on disk could
  be considered a *very simple* database, but
  we usually mean much more advanced programs.

.. _`relational database`:

Relational database
  A very common kind of database that's good
  at retrieving data that have relationships
  to one another.  For instance, a question like
  "How expensive is the cat food brand that most
  of my cats prefer?" is usually easier to answer
  in a relational database than in other types
  of database.

RDBMS
  Relational database management system - basically
  a synonym for `relational database`.

SQL
  The specialized language usually used to get
  and manipulate data in a `relational database`_.

SQL database
  More or less a synonym for `relational database`_.

.. _`non-relational database`:
  An alternative to a `relational database`.  It's
  generally easier to use and often faster to run,
  but has its own disadvantages for complex kinds
  of data access.

.. `NoSQL database`:
  More or less a synonym for `non_relational database`_.

Techniques
----------

.. _`version control`:

Version Control
  Tools and techniques for keeping track of the
  changes in files in a reversible way.  More
  importantly, it helps people cooperate on
  changes to a file without ruining each others'
  work.

Testing
  To programmers, them means scripts that verify
  that a program works

Regression test
  Tests to make sure that one part of a program
  doesn't get worse - *regress* - as improvements
  aren't made to a different part.  All of our
  tests could generally be considered regression
  tests.

.. _`unit test`:

Unit Test
  A fine-scale test that works directly on one small
  piece
  of a program, at a scale finer than the end-user
  will directly see.  Contrast `functional test`_.

.. _`functional test`:

Functional test
  A test that makes sure a program is working from
  the user's point of view.  Contrast `unit test`_.

Test-Driven Development
  A style of development where you first write the
  tests saying what you want the program to do -
  even before the program exists.  Then you write
  the code until the tests no longer fail.

Agile Development
  TODO

Architecture
------------

API
  Shorthand for "application programmer interface".
  This is a way to pass messages back and forth in
  order to add functionality to a program.
  Examples include POSIX (the unix/Linux API), Win32,
  Cocoa, Amazon AWS, and Android. However, many other
  services have APIs to add things like (for instance)
  Dropbox and Facebook to your app.

  TODO: generalize this more

Deploy
  To deliver a completed program so that other
  people can use it. Ususually different than
  just programming it so that it works. Sometimes,
  a program needs to be installed in a package,
  or through an App Store, or maybe it just needs to
  be on the web. That last step to make it so that
  other people can reach it is called "deployment"

Continuous Integration
  TODO
