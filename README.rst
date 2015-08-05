python_learners_glossary
========================

Definitions of Python jargon to help Python beginners
understand Pythonista gobbletigook.  The idea is to
help a Python beginner's understanding even before
they've learned to write the code.

CONTRIBUTING
============

Please submit issues_ and `pull requests`_!

1. Clarity
2. Conciseness
3. Accuracy

... are all desirable - *in that order*.
Don't get pedantic or hung up on `corner cases`_.

Terms to define are not strictly Python terms,
but any terms likely to be frequently heard at
a Python conference.

To reduce cognitive load, let's use examples around
a consistent, familiar theme: cats.

Glossary
========

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

.. _literal:

Literal
  A representation of a value *as the value itself*, as
  opposed to the result of a function_ or expression_.

  ::

    "Whiskers"  # a string literal
    'Whiskers'  # a string literal
    1  # an integer literal
    1.5  # a float literal
    ["Whiskers", 10]  # a list literal

String
  A piece of text data, like ``'hello'``.  Enclosing it
  in quotation marks
  tells Python that it's a string and not something like
  a variable_ name.

Float
  Short for *floating-point number*, a number with a
  decimal point.

.. _variable:

Variable
  A piece of data that has a name.

  ::

      cat_name = 'Fluffy'

  Now ``cat_name`` is a *variable* with the value_ 'Fluffy'.

Assign
  Give a name to a value_, making a variable_.

.. _expression:

Expression
  A description of a value that contains
  calculations and/or
  other executable code; the code must be
  executed to determine the expression's
  actual value.  Typically,
  these fit on one line, but not necessarily.

  Examples::

      'lazy ' + 'cat'  # Evaluates to 'lazy cat'
      2 * 2 > 100  # Evaluates to ``False``

Boolean
  ``True`` or ``False``.

.. _list:

List
  A series of values.  Python will remember what order they
  come in.

  ::

      ['Mouser', 17, 'Whiskers']

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
  A logical grouping of functions (called "methods_"
  in this context) and variables
  (called "attributes_" in this context).

.. _method:
.. _methods:

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
.. attributes_:

Attribute
  A piece of data that belongs to an object.
  This object, ``my_cat``, has a ``name`` attribute
  with the value ``'Agamemnon'``.``

  ::

      my_cat.name
      'Agamemnon'

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

`Object-oriented programming`_
  Programming that makes use of classes_ and objects_.

Dunder
  The two underscores before and after a method name to
  indicate that it is "magic", i.e. __init__, __new__, etc.
  (Short for "Double-underscore")

Magic Method
  Methods that can be used to change the normal
  behavior of an object. HINT : in Python, everything is an object.

Program Structure
-----------------

.. _module:

`Module`_
  A single file of Python commands.  Calling it a
  module implies we plan to "import" it, not just
  call it on its own.

.. _package:

`Package`_
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

`IDE`_
  Abbreviation for Integrated Development Environment.
  A kind of text editor_ with programming-related
  superpowers; a program that lets you build more programs.
  Examples include Eclipse, Sublime, Wingware, and IDLE

`Database`_
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

REPL
  TODO

Techniques
----------

.. _bug:
.. _bugs:

Bug
  A mistake in software that makes it crash or
  behave badly.

Debug
  Fix bugs_

Refactor
  Change a program so that the functionality seems
  the same from the user's point of view, but the
  code itself is better - easier to read, understand,
  maintain, etc.

Agile Development
  TODO

Version Control
---------------

Version Control
  Tools and techniques for keeping track of the
  changes in files in a reversible way.  More
  importantly, it helps people cooperate on
  changes to a file without ruining each others'
  work.

.. _issue:
.. _issues:

Issue
  Request for a specific change to software,
  either to fix a bug_ or provide new features
  ("enhancement").  Issues are usually filed
  in a project's `bug tracker`_.

Bug report
  A category of issue_ for notifying the programmers
  of a bug_

.. _repository:
.. _repositories:

Repository
  A record on disk of the `version control`_ history
  for a directory (and its subdirectories).  Usually
  we mean someplace on line, usually at a service like
  github_.

Repo
  Abbreviation for repository_.

Branch
  TODO

.. _fork:

Fork
  TODO

.. _pull request:
.. _pull requests:

Pull Request
  After you have fork_ed a repository_ and made
  changes, you may ask the original repository
  owner to incorporate ("pull") your changes into the
  original repository.

Git
  The most popular program for version control.

Mercurial
  Another version control program

Github
  The most popular commercial service that
  hosts version control
  repositories_ online.

Bitbucket
  Another commercial service for hosting version
  control repositories_.

Testing
-------

Testing
  To programmers, them means scripts that verify
  that a program works as desired automatically.
  We rarely talk about non-automated, direct human
  testing, because it's soul-sucking and can't keep
  up with our speed of generating bugs_.

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

Corner Case
  A situation that's likely to show bugs_ in code
  because it's so unusual that the developers were
  unlikely to account for it.  For instance, if you
  are classifying cats by their eye color, a cat with
  two different-color eyes may be a corner case that
  disrupts your classification scheme.

Packaging
---------

PyPI
  `PyPI <https://pypi.python.org/pypi>`_, pronounced "Pie-Pee-Eye" and also
  known as *The Cheeseshop*, is the "Python Packaging Index".
  It is where you can publish and download open source Python packages.

pip
  `pip <https://pip.pypa.io/en/latest/index.html>`_ is the recommended tool
  for installing Python packages and is preferred over
  `easy_install <https://pypi.python.org/pypi/setuptools>`_.

Architecture
------------

API
  Shorthand for "application programmer interface".
  This is the way that other programs can make use
  of this program.  Web services can have APIs that
  let them accept messages from other programs and send
  messages back in response.

  Examples include POSIX (the unix/Linux API), Win32,
  Cocoa, Amazon AWS, and Android. However, many other
  services have APIs to add things like (for instance)
  Dropbox and Facebook to your app.

  TODO: generalize this more

Operations
----------

Operations
  Activities related to deploy_ing software and
  keeping it running on its destination servers.

DevOps
  Philosophy and tools for operations_ that try to
  make the process as automatic and failsafe as
  possible by imitating software developers' tools
  and techniqes.

.. _deploy:

Deploy
  To deliver a completed program so that other
  people can use it. Ususually different than
  just programming it so that it works. Sometimes,
  a program needs to be installed in a package,
  or through an App Store, or maybe it just needs to
  be on the web. That last step to make it so that
  other people can reach it is called "deployment"

Build
  TODO

Build Server
  TODO

`Continuous Integration`_
  TODO

More words to define
--------------------

GIL
  TODO
  
PEP
  TODO
  
PEP 8
  TODO
  
program
  TODO
  
script
  TODO
  
scripting language
  TODO
  
regex
  TODO
  
pickle
  TODO
  
socket
  TODO
  
thread
  TODO
  
virtualenv
  TODO
  
kit
  TODO
  
hash
  TODO
  
commit
  TODO
  
branch
  TODO
  
polymorphism
  TODO
  
inheritance
  TODO
  
bytecode
  TODO
  
serialize
  TODO
  
JSON
  TODO
  
YAML
  TODO
  
XML
  TODO
  
HTML
  TODO
  
CSS
  TODO
  
dependency injection
  TODO
  
repr
  TODO
  
queue
  TODO
  
event
  TODO
  
message
  TODO
  
GUI
  TODO
  
command line
  TODO
  
loop
  TODO
  
list comprehension
  TODO
  
lambda
  TODO
  
closure
  TODO
  
generator
  TODO
  
coroutine
  TODO

blocking
  TODO

lock
  TODO
  
mutex
  TODO
  
semaphore
  TODO
  
signal
  TODO
  
bit
  TODO
  
callable
  TODO
  
namespace
  TODO
  
file object
  TODO
  
query
  TODO
  
comment
  TODO
  
code
  TODO
  
cron
  TODO
  
constant
  TODO
  
C API
  TODO
  
utf-8
  TODO
  
ascii
  TODO
  
encoding
  TODO
  
code point
  TODO
  
hex
  TODO
  
binary
  TODO
  
octal
  TODO
  
source
  TODO
  
NLTK
  TODO
  
MVC
  TODO
  
file extension
  TODO
  
functional programming
  TODO
  
higher-order function
  TODO
  
first-class value
  TODO
  
indentation
  TODO
  
SQL injection
  TODO

decorator
  TODO
  
code object
  TODO
  
frame
  TODO
  
traceback
  TODO
  
statement
  TODO
  
standard library
  TODO
  
IDLE
  TODO
  
twisted
  TODO
  
django
  TODO
  
flask
  TODO
  
requests
  TODO
  
scipy
  TODO
  
numpy
  TODO
  
pandas
  TODO
  
matplotlib
  TODO
  
ipython
  TODO
  
jupyter
  TODO
  
setup.py
  TODO
  
mutable
  TODO
  
immutable
  TODO
  
unicode
  TODO
  
byte
  TODO
  
byte string
  TODO
  
array
  TODO
  
CPython
  TODO
  
PyPy
  TODO
  
Jython
  TODO
  
Cython
  TODO
  
ctypes
  TODO
  
cffi
  TODO
  
compile
  TODO
  
interpret
  TODO
  
syntax
  TODO
  
integration test
  TODO
  
load test
  TODO
  
performance test
  TODO
  
acceptance test
  TODO
  
mock
  TODO
  
stub
  TODO
  
fake
  TODO
  
test double
  TODO
  
coverage
  TODO
  
alpha
  TODO
  
beta
  TODO
  
release candidate
  TODO
  
semantic versioning
  TODO
  
sphinx
  TODO
  
ReST
  TODO
  
rst
  TODO
  
documentation
  TODO
  
docstring
  TODO
  
doctest
  TODO
  
concatenation
  TODO
  
slice
  TODO
  
index
  TODO
  
item
  TODO
  
property
  TODO
  
descriptor
  TODO
  
metaclass
  TODO
  
emacs
  TODO
  
vim
  TODO
  
pycharm
  TODO
  
sublime
  TODO
  
exception
  TODO
  
catch
  TODO
  
raise
  TODO
  
error
  TODO
  
CSV
  TODO
  
server
  TODO
  
client
  TODO
  
protocol
  TODO
  
network
  TODO
  
import
  TODO
  
synchronous
  TODO
  
asynchronous
  TODO
  
type
  TODO
  
type checking
  TODO
  
duck typing
  TODO
  
DSL
  TODO
  
subclass
  TODO
  
superclass
  TODO
  
mixin
  TODO
  
multiple inheritance
  TODO
  
interface
  TODO
  
abstract class
  TODO
  
static method
  TODO
  
operating system
  TODO
  
Windows
  TODO
  
Linux
  TODO
  
Ubuntu
  TODO
  
pastebin
  TODO
  
IRC
  TODO
  
operator
  TODO
  
operation
  TODO
  
object-oriented
  TODO
  
use case
  TODO
  
requirements
  TODO
  
recursion
  TODO
  
iteration
  TODO
  
garbage collection
  TODO
  
memory management
  TODO
  
reference
  TODO
  
c extension
  TODO
  
factory
  TODO
  
portable
  TODO
  
pythonic
  TODO
  
singleton
  TODO


.. _`Module`: http://docs.python-guide.org/en/latest/writing/structure/#modules

.. _`Object-oriented programming`: http://docs.python-guide.org/en/latest/writing/structure/#object-oriented-programming

.. _`Continuous Integration`: http://docs.python-guide.org/en/latest/scenarios/ci/

.. _`Database`: http://docs.python-guide.org/en/latest/scenarios/db/

.. _`IDE`: http://docs.python-guide.org/en/latest/dev/env/#ides

.. _`Package`: http://docs.python-guide.org/en/latest/writing/structure/#packages
