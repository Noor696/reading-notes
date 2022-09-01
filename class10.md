## In memory storage

**Reading**

(Understanding the JavaScript Call Stack)[https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4]

**What is a 'call'?**
a call stack is a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation (call).

**How many 'calls' can happen at once?**
It is single-threaded. Meaning it can only do one thing at a time.


**What does LIFO mean?**
Last In, First Out data structure.
LIFO: When we say that the call stack, operates by the data structure principle of Last In, First Out, it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.

**Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.**


**What causes a Stack Overflow?**
A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.



(JavaScript error messages)[https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c]

**What is a 'reference error'?**
when you try to use a variable that is not yet declared

**What is a 'syntax error'?**
this occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.

**What is a 'range error'?**

**What is a 'tyep error'?**
this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.

**What is a breakpoint?**
In the debugger window, you can set breakpoints in the JavaScript code.

At each breakpoint, JavaScript will stop executing, and let you examine JavaScript values.

After examining values, you can resume the execution of code (typically with a play button).


**What does the word 'debugger' do in your code?**
The debugger keyword stops the execution of JavaScript, and calls (if available) the debugging function.
if you want to check your JS code,If the line you selected was run you will be able to see what has happened before that point and you can try and evaluate the next lines to check if everything is outputting what you are expecting.
