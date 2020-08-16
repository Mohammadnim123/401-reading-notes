# Python Modules and Packages – An Introduction

**Python Modules: Overview**

There are actually three different ways to define a module in Python:

1. A module can be written in Python itself.

1. A module can be written in C and loaded dynamically at run-time, like the re (regular expression) module.

1. A built-in module is intrinsically contained in the interpreter, like the itertools module.

**The import Statement**


Module contents are made available to the caller with the import statement. The import statement takes many different forms, shown below.

`import <module_name>`

**The dir() Function**

The built-in function dir() returns a list of defined names in a namespace. Without arguments, it produces an alphabetically sorted list of names in the current local symbol table.

**Executing a Module as a Script**

Any .py file that contains a module is essentially also a Python script, and there isn’t any reason it can’t be executed like one.

**Reloading a Module**

For reasons of efficiency, a module is only loaded once per interpreter session. That is fine for function and class definitions, which typically make up the bulk of a module’s contents. But a module can contain executable statements as well, usually for initialization. Be aware that these statements will only be executed the first time a module is imported.

**Python Packages**

Suppose you have developed a very large application that includes many modules. As the number of modules grows, it becomes difficult to keep track of them all if they are dumped into one location. This is particularly so if they have similar names or functionality. You might wish for a means of grouping and organizing them.

Packages allow for a hierarchical structuring of the module namespace using dot notation. In the same way that modules help avoid collisions between global variable names, packages help avoid collisions between module names.

**Package Initialization**

If a file named `__init__`.py is present in a package directory, it is invoked when the package or a module in the package is imported. This can be used for execution of package initialization code, such as initialization of package-level data.

[video totorial](https://realpython.com/courses/python-modules-packages/)

# Pytest

**pytest: helps you write better programs**

**What is PyTest?**

Pytest is a testing framework which allows us to write test codes using python. You can write code to test anything like database , API, even UI if you want. But pytest is mainly being used in industry to write tests for APIs.

**Why use PyTest?**

_Some of the advantages of pytest are:_

* Very easy to start with because of its simple and easy syntax.
* Can run tests in parallel.
* Can run a specific test or a subset of tests
* Automatically detect tests
* Skip tests
* Open source

# Recursion

**What is Recursion?**
The process in which a function calls itself directly or indirectly is called recursion and the corresponding function is called as recursive function. Using recursive algorithm, certain problems can be solved quite easily.

**How a particular problem is solved using recursion?**

The idea is to represent a problem in terms of one or more smaller problems, and add one or more base conditions that stop the recursion. For example, we compute factorial n if we know factorial of (n-1). The base case for factorial would be n = 0. We return 1 when n = 0.

**Why Stack Overflow error occurs in recursion?**

If the base case is not reached or not defined, then the stack overflow problem may arise. Let us take an example to understand this.

**What is the difference between direct and indirect recursion?**

A function fun is called direct recursive if it calls the same function fun. A function fun is called indirect recursive if it calls another function say fun_new and fun_new calls fun directly or indirectly. 

**How memory is allocated to different function calls in recursion?**

When any function is called from main(), the memory is allocated to it on the stack. A recursive function calls itself, the memory for a called function is allocated on top of memory allocated to calling function and different copy of local variables is created for each function call.