# Python course

## Outline
```
0. Groundwork
  0.0 Introduction
    0.0.X What is Python - high level, usually interpreted, dynamically typed, very readablem multiparadigm programming language.
    0.0.X History: 1989-1991, when first release was published. Python 2.0 - 2000 (PEP, support for unicode, cycle detecting. interpreter). Python 3.0 - 2008.
    0.0.X Who uses python:
      0.0.X.X System / network admins / SREs: launching apps, configuration management, testing (what if application dies) - ansible.
      0.0.X.X Web Devs: API (flask microframework, bottle), feature rich webapps (django, web2py), CMS/ERP (django-cms, mezzanine).
      0.0.X.X Application users: scripting "Blender 3D" and other application scipting.
      0.0.X.X Data Scientists and machine learning professionals. 
      0.0.X.X Scientists.
      0.0.X.X Mobile development.
    0.0.X Popularity: SO questions, PYPL ranking, IEEE Spectrum report, TIOBE index.
    0.0.X PEP 20 and Pythoninc philosophy: focus on readability and software maintainability.
    0.0.X Notes on versions 2.X vs 3.X
      0.0.X.X Not backwards compatible, so many features could be added, use Python3 by default.
      0.0.X.X Package names: python3, pip3, ipython3
    0.0.X Tools: 
      0.0.X.X REPL - read execute print loop.
      0.0.X.X Interpreter: a way to run programms from files.
      0.0.X.X Pip - package manager.
      0.0.X.X Ipython - interactive shell that is more powerfull (autoreload can be enabled nativelly).
      0.0.X.X Pypi - python package index
    0.0.X Documentation:
      0.0.X.X https://www.python.org/
      0.0.X.X https://docs.python.org/3/
  0.1 The Interpreter
    0.1.0 
1. Core Python
  1.0 Simple datatypes
    1.0.0 Numbers
    1.0.1 Strings
      1.0.1.0 Double qoute vs. single qoute
      1.0.1.1 Escape sequences: \n, \t, \\
      1.0.1.2 Multiline strings
      1.0.1.3 Formating w/ print: print(%s), print(s * 5)
      1.0.1.4 Slicing and spliting, stripping whitespace, creating a list from string.
    1.0.2 Lists
      1.0.2.0 Simple operations: creation, assignment, access, looping, sorting, inserting, appending, min, max, len.
      1.0.2.1 Slicing
      1.0.2.2 List comprehensions
      1.0.2.3 Nested lists
    1.0.3 Dictionaries / map: unique key, cant' be joined like lists.
       // get values
       // get keys
       // ... other simple operations
    1.0.4 Tuples: same as list, but static.
  1.1 Simple operators
    1.1.0 Arythmetic
    1.1.1 Logical
    1.1.2 Precedence of operators
  1.1 Control structures
    1.1.0 Branching: if, else, elif
    1.1.1 Looping: for i in range(6), for i in [], while
  1.4 User input
    1.4.0 //
  1.5 Functions - reusable, addresable code:
    1.5.0 Caller and callee: return returns to the caller.
    1.5.1 Scope: don't use global, function-locals not available after function ends.
2. Advanced Python
  2.0 Classes & OO
    2.0.0. //
  2.1 Functional Concepts
    2.1.0. //
  2.2 I/O: Files, Networking, process management (subprocesses and pipes)
    2.2.0. //
  2.3 Exceptions
    2.3.0. //
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
  
```
### Excercises:
- https://www.w3resource.com/python-exercises/
- http://www.practicepython.org/
- https://raw.githubusercontent.com/zhiwehu/Python-programming-exercises/master/100%2B%20Python%20challenging%20programming%20exercises.txt
