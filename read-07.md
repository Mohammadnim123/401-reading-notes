# Python global and nonlocal

**Use global and nonlocal variables. Indicate how variables are referenced in methods.**

>Global, nonlocal. Variable names are sometimes conflicting. In a method, an identifier may reference a local variable or a global variable. The global and nonlocal keywords indicate which variable is being referenced.

> In Python, the notions of global scope and global names are tightly associated with module files. For example, if you define a name at the top level of any Python module, then that name is considered global to the module. That’s the reason why this kind of scope is also called module scope.

This program uses the global keyword. In method(), we use the statement "global value." This means that the identifier "value" refers to the global "value," which is accessed outside the method.

**Result:** The variable is changed to equal 100 in method(). And this is reflected in the global variable at the end of the program.


**Nonlocal.** Nonlocal is similar in meaning to global. But it takes effect primarily in nested methods. It means "not a global or local variable." So it changes the identifier to refer to an enclosing method's variable.

**Global and nonlocal are not needed in many (probably most) Python programs. But, when needed, they make methods conflict less with enclosing methods or the global scope. They make the syntax, however, more complex.**

>The scope of a variable or name defines its visibility throughout your code. In Python, scope is implemented as either a Local, Enclosing, Global, or Built-in scope. When you use a variable or name, Python searches these scopes sequentially to resolve it. If the name isn’t found, then you’ll get an error. This is the general mechanism that Python uses for name resolution and is known as the LEGB rule.

* **Take** advantage of Python scope to avoid or minimize bugs related to name collision.

* **Make** good use of global and local names across your programs to improve code maintainability.

* **Use** a coherent strategy to access, modify, or update names across all your Python code.

