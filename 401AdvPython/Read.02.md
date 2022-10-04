# Read 02 - Testing and Modules

[In Tests We Trust — TDD with Python](https://code.likeagirl.io/in-tests-we-trust-tdd-with-python-af69f47e6932)

**Unit tests and TDD**

_Unit tests_ are some pieces of code to exercise the input, the output and the behaviour of your code. You can write them anytime you want.
_Test-Driven Development_ is a strategy to think (and write!) tests first.

**Important steps to care about is the structure**

**AAA: Arrange, Act and Assert.**

* Arrange: you need to organize the data needed to execute that piece of code (input).
* Act: here you will execute the code being tested (exercise the behaviour);
* Assert: after executing the code, you will check if the result (output).

**The Cycle**

The cycle is made by three steps:
- Write a unit test and make it fail
- Write the feature and make the test pass.
- Refactor the code — the first version doesn’t need to be the beautiful one.

-------------------------

[If name equals main](https://www.geeksforgeeks.org/what-does-the-if-__name__-__main__-do/)

If the python interpreter is running that module (the source file) as the main program using the command "python script.py", it sets the special __name__ variable to have a value “__main__”. If this file is being imported from another module, __name__ will be set to the module’s name. Module’s name is available as value to __name__ global variable. 

Advantages : 
- Every Python module has it’s __name__ defined and if this is ‘__main__’, it implies that the module is being run standalone by the user and we can do corresponding appropriate actions.
- If you import this script as a module in another script, the __name__ is set to the name of the script/module.
- Python files can act as either reusable modules, or as standalone programs.
- if __name__ == “main”: is used to execute some code only if the file was run directly, and not imported.

-------------------------

[Introduction to Recursion](https://www.geeksforgeeks.org/introduction-to-recursion-data-structure-and-algorithm-tutorials/)

**What is Recursion?**
* The process in which a function calls itself directly or indirectly is called recursion and the corresponding function is called a recursive function. Using a recursive algorithm, certain problems can be solved quite easily.

* Recursion is an amazing technique with the help of which we can reduce the length of our code and make it easier to read and write.

* Performing the same operations multiple times with different inputs. In every step, we try smaller inputs to make the problem smaller. Base condition is needed to stop the recursion otherwise infinite loop will occur.

* When any function is called from main(), the memory is allocated to it on the stack. A recursive function calls itself, the memory for a called function is allocated on top of memory allocated to the calling function and a different copy of local variables is created for each function call. When the base case is reached, the function returns its value to the function by whom it is called and memory is de-allocated and the process continues.

-------------------------

[Python Modules and Packages: An Introduction](https://realpython.com/lessons/python-modules-packages-overview/)

Python modules and Python packages, two mechanisms that facilitate modular programming.

Modular programming is the process of breaking a large, unwieldy programming task into separate, smaller, more manageable subtasks or modules. Individual modules can then be put together like building blocks to create a larger application.

**advantages to modularizing code in a large application:**

- Simplicity

- Maintainability

- Reusability

- Scoping


