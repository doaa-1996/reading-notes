# Call stack

A call stack is a mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions — what function is currently being run and what functions are called from within that function, etc.



function greeting() {

   // [1] Some codes here

   sayHi();

   // [2] Some codes here

}

function sayHi() {

   return "Hi!";

}


// Invoke the `greeting` function

greeting();

// [3] Some codes here



At the most basic level, a call stack is a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation (call).

LIFO: When we say that the call stack, operates by the data structure principle of Last In, First Out, it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.

Temporarily store: When a function is invoked (called), the function, its parameters, and variables are pushed into the call stack to form a stack frame. This stack frame is a memory location in the stack. The memory is cleared when the function returns as it is pop out of the stack.


Manage function invocation (call): The call stack maintains a record of the position of each stack frame. It knows the next function to be executed (and will remove it after execution). This is what makes code execution in JavaScript synchronous.


# JavaScript error messages && debugging

***Types of error messages***

***Reference errors***

This is as simple as when you try to use a variable that is not yet declared you get this type of errors.


console.log(foo) // Uncaught ReferenceError: foo is not defined

foo = 'Hello' // Uncaught ReferenceError: foo is not defined


Whatever you are using (var, let or const) the fix is as simple has declaring the variable before any declaration is made.

let foo;

foo = 'Hello'


***Syntax errors***

JSON.parse( {'foo': 'bar'} ) // Uncaught SyntaxError: Unexpected token o in JSON at position 1


This can be solved by just fixing the syntax, in this case the object should be a JSON.

JSON.parse('{"foo":"bar"}')


***Range errors***


Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.


var foo= []
foo.length = foo.length -1 // Uncaught RangeError: Invalid array length