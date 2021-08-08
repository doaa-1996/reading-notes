# Pythonisms

Iterators provide a sequence interface to Python objects that’s memory efficient and considered Pythonic. Behold the beauty of the for-in loop!

To support iteration an object needs to implement the iterator protocol by providing the iter and next dunder methods.

Class-based iterators are only one way to write iterable objects in Python. Also consider generators and generator expressions.

**Python Iterators That Iterate Forever**


We’ll begin by writing a class that demonstrates the bare-bones iterator protocol in Python. The example I’m using here might look different from the examples you’ve seen in other iterator tutorials, but bear with me. I think doing it this way gives you a more applicable understanding of how iterators work in Python.

Over the next few paragraphs we’re going to implement a class called Repeater that can be iterated over with a for-in loop, like so:

repeater = Repeater(‘Hello’) for item in repeater: print(item) Like its name suggests, instances of this Repeater class will repeatedly return a single value when iterated over. So the above example code would print the string Hello to the console forever.

To start with the implementation we’ll define and flesh out the Repeater class first:

```
class Repeater:
    def __init__(self, value):
        self.value = value

    def __iter__(self):
        return RepeaterIterator(self)
```

On first inspection, Repeater looks like a bog-standard Python class. But notice how it also includes the iter dunder method.

What’s the RepeaterIterator object we’re creating and returning from iter? It’s a helper class we also need to define for our for-in iteration example to work:

```
class RepeaterIterator:
    def __init__(self, source):
        self.source = source

    def __next__(self):
        return self.source.value
```


Again, RepeaterIterator looks like a straightforward Python class, but you might want to take note of the following two things:

In the init method we link each RepeaterIterator instance to the Repeater object that created it. That way we can hold on to the “source” object that’s being iterated over.

In RepeaterIterator.next, we reach back into the “source” Repeater instance and return the value associated with it.

In this code example, Repeater and RepeaterIterator are working together to support Python’s iterator protocol. The two dunder methods we defined, iter and next, are the key to making a Python object iterable.

We’ll take a closer look at these two methods and how they work together after some hands-on experimentation with the code we’ve got so far.

Let’s confirm that this two-class setup really made Repeater objects compatible with for-in loop iteration. To do that we’ll first create an instance of Repeater that would return the string ‘Hello’ indefinitely:

repeater = Repeater(‘Hello’) And now we’re going to try iterating over this repeater object with a for-in loop. What’s going to happen when you run the following code snippet?

for item in repeater: … print(item) Right on! You’ll see ‘Hello’ printed to the screen…a lot. Repeater keeps on returning the same string value, and so, this loop will never complete. Our little program is doomed to print ‘Hello’ to the console forever:

Hello Hello Hello Hello Hello … But congratulations—you just wrote a working iterator in Python and used it with a for-in loop. The loop may not terminate yet…but so far, so good!

Next up we’ll tease this example apart to understand how the iter and next methods work together to make a Python object iterable.

Pro tip: If you ran the last example inside a Python REPL session or from the terminal and you want to stop it, hit Ctrl + C a few times to break out of the infinite loop.


**Generators**

Generators use yield statements instead of return. Local variables and the execution state of the generator function are only stashed away temporarily and not thrown out completely. Generators start raising StopIteration exceptions after control flow leaves the generator function by any means other than a yield statement.

