## Read 05 - Intro to OOP

### Classes and Objects

[Classes and Objects](https://www.learnpython.org/en/Classes_and_Objects)

* Objects are an encapsulation of variables and functions into a single entity.
* Objects get their variables and functions from classes.
* Classes are essentially a template to create your objects.
* You can create multiple different objects that are of the same class(have the same variables and functions defined).
* each object contains independent copies of the variables defined in the class. 
* The __init__() function, is a special function that is called when the class is being initiated. It's used for assigning values in a class.


### Thinking Recursively in Python

[Thinking Recursively in Python](https://realpython.com/python-thinking-recursively/)

Problems (in life and also in computer science) can often seem big and scary. But if we keep chipping away at them, more often than not we can break them down into smaller chunks trivial enough to solve. This is the essence of thinking recursively.

* the typical structure of a recursive algorithm. If the current problem represents a simple case, solve it. If not, divide it into subproblems and apply the same strategy to them.

- Recursive Functions in Python: 
A recursive function is a function defined in terms of itself via self-referential expressions.

This means that the function will continue to call itself and repeat its behavior until some condition is met to return a result. All recursive functions share a common structure made up of two parts: base case and recursive case.


### Python Testing with pytest: Fixtures and Coverage

[pytest: Fixtures and Coverage](https://www.linuxjournal.com/content/python-testing-pytest-fixtures-and-coverage)

pytest has become quite popular, in no small part because it's so easy to write tests and integrate those tests into your software development process. I've become a big fan, mostly because after years of saying I should get better about testing my software, pytest finally has made it possible.

**two features of pytest: fixtures and code coverage**

* **Fixtures:**

you define fixtures using a combination of the pytest.fixture decorator, along with a function definition.

* **code coverage:**

Pytest is a fantastic library for writing unit tests. Pytest comes with a built-in feature called code coverage which measures how much code in your project is being tested by your tests.