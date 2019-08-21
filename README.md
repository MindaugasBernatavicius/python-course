# Python course

- Cheatsheets: https://ehmatthes.github.io/pcc/cheatsheets/README.html

## Outline
```
0. Groundwork
  0.0 Introduction
    0.0.X What is Python - high level, usually interpreted, dynamically typed (duck typed), very readable multiparadigm programming language.
    0.0.X History: 1989-1991, when first release was published. Python 2.0 - 2000 (PEP, support for unicode, cycle detecting interpreter). Python 3.0 - 2008.
    0.0.X Who uses python:
      0.0.X.X System / network admins / SREs: launching apps, configuration management, testing (what if application dies) - ansible.
      0.0.X.X Web Devs: API (flask microframework, bottle), feature rich webapps (django, web2py), CMS/ERP (django-cms, mezzanine).
      0.0.X.X Application users: scripting "Blender 3D" and other application scipting.
      0.0.X.X Data Scientists and machine learning professionals (Keras, Tensorflow, PyTorch). 
      0.0.X.X Scientists (Numpy ans Scipy).
      0.0.X.X Mobile development.
      0.0.X.X Desktop development.
    0.0.X Popularity: SO questions, PYPL ranking, IEEE Spectrum report, TIOBE index.
    0.0.X PEP 20 and Pythoninc philosophy: focus on readability and software maintainability.
    0.0.X Notes on versions 2.X vs 3.X
      0.0.X.X Not backwards compatible, so many features could be added, use Python3 by default.
      0.0.X.X Package names: python3, pip3, ipython3
      0.0.X.X Ascii strings in Python2, Unicode strins in Python3.
      0.0.X.X Print was a statement in Python2, in Python3 it's a function.
      0.0.X.X Some new features were added like: TODO.
    0.0.X Tools: 
      0.0.X.X REPL - read execute print loop.
      0.0.X.X Interpreter: a way to run programms from files.
      0.0.X.X Pip - package manager.
      0.0.X.X Ipython - interactive shell that is more powerfull (autoreload can be enabled nativelly).
      0.0.X.X Pypi - python package index
      0.0.X.X Venv - virtual env to keep python executable w/ asociated packages separatelly for different projects.
    0.0.X Documentation:
      0.0.X.X https://www.python.org/
      0.0.X.X https://docs.python.org/3/
  0.1 There are several implementations of python
    0.1.0 CPython
    0.1.1 JPython
    0.1.2 Iron Python, PyPy (small)
  0.2 The Interpreter and installation
    0.2.0 Install
    - REPL, the _ (underscore) in REPL.
    - Other tools like jdoodle (you can create a file there).
    
    
    f = open("guru99.txt","w+")
    f.write("AAAA")
    f.close()

    f = open("guru99.txt", "r+")
    print(f.read())
    f.close()
    
1. Core Python
  1.0 Simple datatypes
    1.X.X Dynamic typing and it's problems (no compile time safety).
    1.0.0 Numbers: int, float and their operations. Complex types.
    1.0.1 Strings
      1.0.1.0 Double qoute vs. single qoute vs. tripple qoute: 'a' == "a" == '''a'''
      1.0.1.1 Escape sequences: \n, \t, \\
      1.0.1.2 Multiline strings
      1.0.1.3 Formating w/ print: print(%s), print(s * 5), "'.format(var1, ...)., f"Hello {name}".
      1.0.1.4 Slicing and spliting, stripping whitespace, creating a list from string.
    1.0.2 Lists
      1.0.2.0 Simple operations: creation, assignment, access, looping, sorting, inserting, appending, min, max, len.
      1.0.2.1 Slicing: list[2:], list[:2], list[2:5]
      1.0.2.2 List comprehensions
      1.0.2.3 Nested lists
    1.1 Control structures
      1.1.0 Branching: if, else, elif
      1.1.1 Looping: for i in range(6), for i in [], while
    1.0.3 Dictionaries / map: unique key, can't be joined like lists.
      1.X.X CRUD and other operations.
    1.0.4 Tuples: same as list, but static.
  1.1 Simple operators
    1.1.0 Arythmetic
    1.1.1 Logical
    1.1.2 Precedence of operators
  1.4 User input
    1.4.0 //
  1.5 Functions - reusable, addresable code:
    X.X.X General form of a function;
    X.X.X Side effects (I/O boundary) and pure functions.
    1.5.0 Caller and callee: return returns to the caller;
    1.5.1 Scope: don't use global, function-locals not available after function ends.
    
      glob = "AAA"

      def print_global():
          # global glob
          glob = "BBB"
          print(glob)

      print(glob)
      print_global()
      print(glob)
    
    X.X.X A function needs to be small and do one thing or at least perform related things.
    X.X.X Function calling another function.
    X.X.X Function calling itself: factorial(), fibonacci(), analysing recursive functions (stacks and tree representations). 
    
2. Advanced Python
  2.0 Classes & OO
    2.0.0. //
  2.1 Functional Concepts
    2.1.0. //
  2.2 I/O: Files, Networking, process management (subprocesses and pipes)
    2.2.0. //
  2.3 Exceptions
    2.3.0 KeyError when no key in disc.
    X.X.X Wrong permissions for a file.
    X.X.X Try-except-else-finally
    X.X.X Exceptions walk the stack, but have no costs when not thrown.
    X.X.X Which code should be wrapped: not in memory (IO operations).
    X.X.X Multi-catch blocks.
  2.4 Testing
    2.4.0. //
    
3. Common applications
  3.0 Scripting and tooling
    3.0.0 Calling an API w/ urllib.
  3.1 GUI programming
    3.1.0 //
  3.2 Data Visualization
    3.2.0 Drawing graphs w/ matplotlib.
  3.3 Simple machine learning
    3.3.0 //
  3.4 Web apps
    3.4.0 Intro to Django
    3.4.1 Interacting w/ DBs
    3.4.2 Templating engines in python
    3.4.3 Doing the same w/ Flask
    
4. Python ecosystems and tools:
  4.X Venv: 
    4.X.X virtualenv project_venv
    4.X.X which pip, which python, pip list - will show which venv you are in
    4.X.X deactivate +> rm -rf project_venv
  4.X Most common packages:
    4.X.X 
    Requests
    Numpy
    Pandas
    Matplotlib
    Scikit-learn
    Tensorflow
    PyQT
    PyGTK
    Scapy
    Scrapy
    Nltk
    Flask
    Django
```
### Excercises:
- https://www.w3resource.com/python-exercises/
- http://www.practicepython.org/
- https://raw.githubusercontent.com/zhiwehu/Python-programming-exercises/master/100%2B%20Python%20challenging%20programming%20exercises.txt
