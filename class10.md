# Error Handling & Debugging


 This chapter will help you learn
how to find the errors in your code. It will also teach you how
to write scripts that deal with potential errors gracefully. 



**ORDER OF EXECUTION** 

To find the source of an error, it helps to know how scripts are processed.
The order in which statements are executed can be complex; some tasks
cannot complete until another statement or function has been run: 


**EXECUTION CONTEXTS** 

The JavaScript interpreter uses the concept of execution contexts.
There is one global execution context; plus, each function creates a new
new execution context. They correspond to variable scope. 




**EXECUTION CONTEXT**

JavaScript
Hello Molly
Every statement in a script lives in one of three
execution contexts:

**Q GLOBAL CONTEXT**

Code that is in the script, but not in a function.
There is only one global context in any page.

**FUNCTION CONTEXT**

Code that is being run within a function.
Each function has its own function context.

**Q EVAL CONTEXT (NOT SHOWN)**

Text is executed like code in an internal function
called eva l {) (which is not covered in this book).


**VARIABLE SCOPE**

The first two execution contexts correspond with the
notion of scope (which you met on p98):

**Q GLOBAL SCOPE**

If a variable is declared outside a function, it can
be used anywhere because it has global scope.
If you do not use the var keyword when creating
a variable, it is placed in global scope.

**FUNCTION-LEVEL SCOPE**

When a variable is declared within a function,
it can only be used within that function. This is
because it has function-level scope. 



**EXECUTION CONTEXT & HOISTING**

Each time a script enters a new execution context, there are two phases
of activity: 


**1: PREPARE**

• The new scope is created
• Variables, functions, and arguments are created
• The value of the this keyword is determined


**2: EXECUTE**

• Now it can assign values to variables
• Reference functions and run their code
• Execute statements


**UNDERSTANDING SCOPE** 



In the interpreter, each execution context has its own va ri ables object.
It holds the variables, functions, and parameters available within it.
Each execution context can also access its parent's v a ri ables object. 



**UNDERSTANDING ERRORS** 


If a JavaScript statement generates an error, then it throws an exception.
At that point, the interpreter stops and looks for exception-handl ing code.



**ERROR OBJECTS** 


Error objects can help you find where your mistakes are
and browsers have tools to help you read them. 


These two pages show JavaScript's seven different types of error objects
and some common examples of the kinds of errors you are likely to see.
As you can tell, the errors shown by the browsers can be rather cryptic. 


**HOW TO DEAL WITH ERRORS**


Now that you know what an error is and how the browser treats them,
there are two things you can do with the errors. 




**1: DEBUG THE SCRIPT TO FIX ERRORS**


If you come across an error while writing a script
(or when someone reports a bug), you will need to
debug the code, track down the source of the error,
and fix it. 


**2: HANDLE ERRORS GRACEFULLY**

You can handle errors gracefully using try, catch,
throw, and f i na 1 ly statements.


**A DEBUGGING WORKFLOW**
Debugging is about deduction: eliminating potential causes of an error




**BROWSER DEV TOOLS & JAVASCRIPT CONSOLE** 


The JavaScript console will tell you when there is a problem with a script,
where to look for the problem, and what kind of issue it seems to be. 




The JavaScript console is just one of several developer tools that are
found in all modern browsers. 


**HOW TO LOOK AT ERRORS IN CHROME** 




The console will show you when there is an
error in your JavaScript. It also displays the line
where it became a problem for the interpreter. 







**TYPING IN THE CONSOLE IN CHROME** 


You can also just type code into the console
and it will show you a result. 




**BREAKPOINTS**


You can pause the execution of a script on any
line using breakpoints. Then you can check the
values stored in variables at that point in time. 




**STEPPING THROUGH CODE** 

If you set multiple breakpoints, you can step
through them one-by-one to see where values
change and a problem might occur.



**CONDITIONAL BREAKPOINTS** 


You can indicate that a breakpoint should be
triggered only if a condition that you specify is
met. The condition can use existing variables. 




**THROWING ERRORS**

If you know something might cause a problem for your script, you can
generate your own errors before the interpreter creates them.






 

