# The global Statement


You already know that when you try to assign a value to a global name inside a function, you create a new local name in the function scope. To modify this behavior, you can use a global statement. With this statement, you can define a list of names that are going to be treated as global names.

The statement consists of the global keyword followed by one or more names separated by commas. You can also use multiple global statements with a name (or a list of names). All the names that you list in a global statement will be mapped to the global or module scope in which you define them.


Here’s an example where you try to update a global variable from within a function:


```
>>> counter = 0  # A global name
>>> def update_counter():
...     counter = counter + 1  # Fail trying to update counter
...
>>> update_counter()
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
  File "<stdin>", line 2, in update_counter
UnboundLocalError: local variable 'counter' referenced before assignment
```


When you try to assign counter inside update_counter(), Python assumes that counter is local to update_counter() and raises an UnboundLocalError because you’re trying to access a name that isn’t defined yet.

If you want this code to work the way you expect here, then you can use a global statement as follows:


```
>>> counter = 0  # A global name
>>> def update_counter():
...     global counter  # Declare counter as global
...     counter = counter + 1  # Successfully update the counter
...
>>> update_counter()
>>> counter
1
>>> update_counter()
>>> counter
2
>>> update_counter()
>>> counter
3
```

In this new version of update_counter(), you add the statement global counter to the body of the function right before you try to change counter. With this tiny change, you’re mapping the name counter in the function scope to the same name in the global or module scope. From this point on, you can freely modify counter inside update_counter(). All the changes will reflect in the global variable.

With the statement global counter, you’re telling Python to look in the global scope for the name counter. This way, the expression counter = counter + 1 doesn’t create a new name in the function scope, but updates it in the global scope.


Note: The use of global is considered bad practice in general. If you find yourself using global to fix problems like the one above, then stop and think if there is a better way to write your code.

For example, you can try to write a self-contained function that relies on local names rather than on global names as follows:


```
>>> global_counter = 0  # A global name
>>> def update_counter(counter):
...     return counter + 1  # Rely on a local name
...
>>> global_counter = update_counter(global_counter)
>>> global_counter
1
>>> global_counter = update_counter(global_counter)
>>> global_counter
2
>>> global_counter = update_counter(global_counter)
>>> global_counter
3
```


This implementation of update_counter() defines counter as a parameter and returns its value augmented by 1 unit every time the function is called. This way, the result of update_counter() depends on the counter you use as an input and not on the changes that other functions (or pieces of code) can perform on the global variable, global_counter.


You can also use a global statement to create lazy global names by declaring them inside a function. Take a look at the following code:
```
>>> def create_lazy_name():
...     global lazy  # Create a global name, lazy
...     lazy = 100
...     return lazy
...
>>> create_lazy_name()
100
>>> lazy  # The name is now available in the global scope
100
>>> dir()
['__annotations__', '__builtins__',..., 'create_lazy_name', 'lazy']
```

# The nonlocal Statement

Similarly to global names, nonlocal names can be accessed from inner functions, but not assigned or updated. If you want to modify them, then you need to use a nonlocal statement. With a nonlocal statement, you can define a list of names that are going to be treated as nonlocal.

The nonlocal statement consists of the nonlocal keyword followed by one or more names separated by commas. These names will refer to the same names in the enclosing Python scope. The following example shows how you can use nonlocal to modify a variable defined in the enclosing or nonlocal scope:

```
>>> def func():
...     var = 100  # A nonlocal variable
...     def nested():
...         nonlocal var  # Declare var as nonlocal
...         var += 100
...
...     nested()
...     print(var)
...
>>> func()
200
```


With the statement nonlocal var, you tell Python that you’ll be modifying var inside nested(). Then, you increment var using an augmented assignment operation. This change is reflected in the nonlocal name var, which now has a value of 200.

Unlike global, you can’t use nonlocal outside of a nested or enclosed function. To be more precise, you can’t use a nonlocal statement in either the global scope or in a local scope. Here’s an example:

```
>>> nonlocal my_var  # Try to use nonlocal in the global scope
  File "<stdin>", line 1
SyntaxError: nonlocal declaration not allowed at module level
>>> def func():
...     nonlocal var  # Try to use nonlocal in a local scope
...     print(var)
...
  File "<stdin>", line 2
SyntaxError: no binding for nonlocal 'var' found
```


In contrast to global, you can’t use nonlocal to create lazy nonlocal names. Names must already exist in the enclosing Python scope if you want to use them as nonlocal names. This means that you can’t create nonlocal names by declaring them in a nonlocal statement in a nested function. Take a look at the following code example:

```
>>> def func():
...     def nested():
...         nonlocal lazy_var  # Try to create a nonlocal lazy name
...
  File "<stdin>", line 3
SyntaxError: no binding for nonlocal 'lazy_var' found
```

In this example, when you try to define a nonlocal name using nonlocal lazy_var, Python immediately raises a SyntaxError because lazy_var doesn’t exist in the enclosing scope of nested().

