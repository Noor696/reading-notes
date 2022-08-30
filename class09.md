## Functional Programming

**Reading**

(Functional Programming Concepts)[https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa]

**What is functional programming?**
 functional programming is a programming paradigm where programs are constructed by applying and composing functions. It is a declarative programming paradigm in which function definitions are trees of expressions that map values to other values, rather than a sequence of imperative statements which update the running state of the program.

**What is a pure function and how do we know if something is a pure function?**

It does not cause any observable side effects,
It returns the same result if given the same arguments.

**What are the benefits of a pure function?**
Pure functions are stable, consistent, and predictable. Given the same parameters, pure functions will always return the same result. We don’t need to think of situations when the same parameter has different results — because it will never happen.

**What is immutability?**
Unchanging over time or unable to be changed.
When data is immutable, its state cannot change after it’s created, Instead, you create a new object with the new value.

**What is Referential transparency?**
a function consistently yields the same result for the same input, it is referentially transparent.

> pure functions + immutable data = referential transparency



**Videos**
(Node JS Tutorial for Beginners #6 - Modules and require)[https://www.youtube.com/watch?v=xHLd36QoS4k]

**What is a module?**
A module is a function or group of similar functions. They are grouped together within a file and contain the code to execute a specific task when called into a larger application.

You create modules to better organize and structure your codebase. You can use them to break down large programs into smaller, more manageable, and more independent chunks of code which carry out a single or a couple of related tasks.


**What does the word ‘require’ do?**
In order to use Node.js core or NPM modules, you first need to import it using require() function as shown below.

> var module = require('module_name');

As per above syntax, specify the module name in the require() function. The require() function will return an object, function, property or any other JavaScript type, depending on what the specified module returns.
**How do we bring another module into the file the we are working in?**
using require('path') in the place we want to use it


**What do we have to do to make a module available?**
You can install third-party modules globally or locally in your project.

Examples of third party modules are express, mongoose, react, etc.

Importing Third-Party Modules

To import a third-party module, you have to use the require() method that takes the third-party module’s name as an argument.

>const fileSystem = require("express");
_____________
In JavaScript, we use the import and export keywords to share and receive functionalities respectively across different modules.

* The export keyword is used to make a variable, function, class or object  accessible to other modules. In other words, it becomes a public code.
* The import keyword is used to bring in public code from another module.
__________

## References
_______

[https://www.freecodecamp.org/](https://www.freecodecamp.org/news/javascript-modules-explained-with-examples/)
[https://www.tutorialsteacher.com/](https://www.tutorialsteacher.com/nodejs/nodejs-modules)