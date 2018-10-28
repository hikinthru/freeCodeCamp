---
title: Python
---

## Python

[Python](https://www.python.org) is a general purpose programming language which is dynamically typed, interpreted, and known for its easy readability with great design principles.

To learn more about Python, check out these pages on python.org:

[What is Python?](https://www.python.org/doc/essays/blurb/)

[Python FAQ](https://docs.python.org/3/faq/general.html)

### Python 2 or Python 3

Python 3 was released on [December 3, 2008](https://www.python.org/download/releases/3.0/). The two versions are similar, with knowledge of one, switching to write code for the other is not difficult. Three changes most commonly encountered in going from 2.x to 3.x are the `print()` function (it is now a function and requires parentheses), the `input()` function (is no longer `raw_input()`), and integer division (Python 3 no longer floors this operation but always creates a float). A full list of changes can be found here. Other considerations include:
 
  * [Python 2.x will not be maintained past 2020](https://www.python.org/dev/peps/pep-0373/)
  * 3.x is under active development. This means that all recent standard library improvements, for example, are only available by default in Python 3.x.
  * The Python ecosystem has amassed a significant amount of quality software over the years. The downside of breaking backwards compatibility in 3.x is that some of that software (especially in-house software in companies) still doesn't work on 3.x yet.

For more information see [Python 2 or Python 3](https://wiki.python.org/moin/Python2orPython3)

### Installation

Most *nix based operating systems (including Macs) come with Python installed (today usually Python 3.x). Replacing a system’s native Python is not recommended and may cause problems because the version installed could be being used for some necessary internal services or tools. However, different versions of Python can be safely installed alongside the system Python. See [Python Setup and Usage](https://docs.python.org/3/using/index.html).

Windows doesn't typically come with Python, the installer and instructions can be found [here](https://docs.python.org/3/using/windows.html).

### The Python Interpreter

The Python interpreter is what is used to run Python scripts, it translates Python code for the operating system.

If it is available and within the Unix shell’s search path it can be started in interactive mode by typing the command `python` (or `python3`, etc. depending on your version and how it was installed). 

To execute a script this would be followed by the script name to invoke the interpreter and run the script.

`hello_campers.py`

```python
print('Hello campers!')
```

From terminal:

```bash
$ python hello_campers.py
Hello campers!
```

When multiple versions of Python are installed, calling them by version is possible depending on the install configuration. In the Cloud9 IDE custom environment, they can be invoked like:

```bash
    $ python --version
    Python 2.7.6
    $ python3 --version
    Python 3.4.3
    $ python3.5 --version
    Python 3.5.1
    $ python3.6 --version
    Python 3.6.2 
    $ python3.7 --version
    Python 3.7.1
```

### Python Interpreter Interactive Mode

Interactive mode can be started by invoking the Python interpreter with the `-i` flag or without any arguments.

Interactive mode provides a prompt where Python commands can be entered and run, this is commonly used for learning Python or trying out statements:

```bash
$ python3.5
Python 3.5.1 (default, Dec 18 2015, 00:00:00)
GCC 4.8.4 on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> print("Hello campers!")
Hello campers!
>>> 1 + 2
3
>>> exit()
$
```

There are many common applications for interactive Python including the one built in to your Python version, available at the command prompt by invoking the version name, as well downloadable applications such as Idle, Spyder and many more.

### The Zen of Python

Some of the principles that influenced the design of Python were written down by Tim Peters, a major contributor to Python's development. The list is included as an Easter egg in Python Interpreters and can be shown by using the following command inside any Python interpreter in interactive mode: `import this`:

    >>> import this
    The Zen of Python, by Tim Peters

    Beautiful is better than ugly.
    Explicit is better than implicit.
    Simple is better than complex.
    Complex is better than complicated.
    Flat is better than nested.
    Sparse is better than dense.
    Readability counts.
    Special cases aren't special enough to break the rules.
    Although practicality beats purity.
    Errors should never pass silently.
    Unless explicitly silenced.
    In the face of ambiguity, refuse the temptation to guess.
    There should be one-- and preferably only one --obvious way to do it.
    Although that way may not be obvious at first unless you're Dutch.
    Now is better than never.
    Although never is often better than *right* now.
    If the implementation is hard to explain, it's a bad idea.
    If the implementation is easy to explain, it may be a good idea.
    Namespaces are one honking great idea -- let's do more of those!

### Pros and Cons of Python

#### Pros
1. Interactive language with module support for almost all functionality.
2. Open Source: So, you can contribute to the community, the functions you have developed for future use can be used to help others.
3. A lot of good interpreters and notebooks available for better experience like Jupyter Notebook.
4. It is a very easy language to learn and debug too. To check if a small bit of code works or not, you can just open up the interpreter and test.

#### Cons

1. Being open source, many different ways have developed over the year for the same function. This sometimes, creates chaos for others to read someone else’s code.
2. It can be a slow language in some implementations because it is interpreted. This can be a deficit for developing some general algorithms.

### Documentation

[Python is well documented](https://docs.python.org/3/). These docs include tutorials, guides, references and meta information for language.

Another important reference is the Python Enhancement Proposals [PEPs](https://www.python.org/dev/peps/). Included in the PEPs is a style guide for writing Python code, [`PEP 8`](https://www.python.org/dev/peps/pep-0008/).

### Debugging

Inline `print` statements can be used for simple debugging:

> **... often the quickest way to debug a program is to add a few print statements to the source: the fast edit-test-debug cycle makes this simple approach very effective.**
> 
> --[Executive Summary](https://www.python.org/doc/essays/blurb/)

Python also includes more powerful tools for debugging, such as:

* logging module, [_logging_](https://docs.python.org/3/library/logging.html)
* debugging module, [_pdb_](https://docs.python.org/3/library/pdb.html)

Just note that these exist for now.

### A Hello World Exercise 

Going back to the docs, we can read about the [`print`](https://docs.python.org/3/library/functions.html#print) function, a ['nofollow'](https://docs.python.org/3/library/functions.html) of the [Python Standard Library](https://docs.python.org/3/library/index.html.

    print(*objects, sep=' ', end='\n', file=sys.stdout, flush=False)

The built-in functions are listed in alphabetical order. The name is followed by a parenthesized list of formal parameters with optional default values. Under that is a short description of the function and its parameters are given and occasionally an example.

The [`print`](https://docs.python.org/3/library/functions.html#print) function in Python 3 replaces the [`print`](https://docs.python.org/2/reference/simple_stmts.html#print) statement in Python 2.

    >>> print("Hello world!")
    Hello world!

A function is called when the name of the function is followed by `()`. For the Hello world! example, the print function is called with a string as an argument for the first parameter. For the rest of the parameters the defaults are used.

The argument that we called is the `print` function which is a `str` object or _string_, one of Python's [_built-in types_](https://docs.python.org/3/library/stdtypes.html#text-sequence-type-str).
Also the most important thing about python is that you don't have to specify the data type while declaring a variable, python's compiler will do that itself based on the type of value assigned.

The `objects` parameter is prefixed with a `*` which indicates that the function will take an arbitrary number of arguments for that parameter.

### Things You Can Do With Python

As stated python is a general purpose language. You can use it to do anything you like, but one of the major uses of python is in machine learning and artificial intelligence. It is also a popular language in Web development with some amazing frameworks like [Django](https://www.djangoproject.com/) and [Flask](http://flask.pocoo.org/). It is also a popular scripting language. With its easy to read syntax it is becoming one the most popular programming languages and is growing rapidly in many fields.

### Learn More

Free Code Camp has some great resources. The web is a big place, there's plenty more to explore:
* [Python Practice Book](http://anandology.com/python-practice-book/index.html)
* [Think Python](http://greenteapress.com/thinkpython/html/index.html)
* [Practical Business Python](http://pbpython.com/)
* [Another course](https://realpython.com/?utm_source=fsp&utm_medium=promo&utm_campaign=bestresources)
* [General](https://www.fullstackpython.com/)
* [Learn the Basics](https://www.codecademy.com/learn/learn-python)
* [Computer science using Python](https://www.edx.org/course/introduction-computer-science-mitx-6-00-1x-11?ref=hackernoon#!)
* [Another computer science course using Python](https://www.udacity.com/course/intro-to-computer-science--cs101)
* [List of more resources for learning Python](https://github.com/vinta/awesome-python)
* [Interactive Python](http://interactivepython.org/runestone/static/thinkcspy/index.html)
* [Developer's Guide to Python](https://devguide.python.org/)
* [Learn Python the Hard Way book](https://learnpythonthehardway.org/python3/)
* [Introduction to Python Programming](https://www.udacity.com/course/introduction-to-python--ud1110)
