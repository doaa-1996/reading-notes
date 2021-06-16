# Stacks and Queues

## What is a Stack


A stack is a data structure that consists of Nodes. Each Node references the next Node in the stack, but does not reference its previous.


Common terminology for a stack is

1. Push - Nodes or items that are put into the stack are pushed.

2. Pop - Nodes or items that are removed from the stack are popped. When you attempt to pop an empty stack an exception will be raised.

3. Top - This is the top of the stack.

4. Peek - When you peek you will view the value of the top Node in the stack. When you attempt to peek an empty stack an exception will be raised.

5. IsEmpty - returns true when stack is empty otherwise returns false.


Stacks follow these concepts:

**FILO**

First In Last Out

This means that the first item added in the stack will be the last item popped out of the stack.

**LIFO**

Last In First Out

This means that the last item added to the stack will be the first item popped out of the stack.



**Stack Visualization**


Here’s an example of what a stack looks like. As you can see, the topmost item is denoted as the top. When you push something to the stack, it becomes the new top. When you pop something from the stack, you pop the current top and set the next top as top.next


![m](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/images/stack1.PNG)



## What is a Queue

**Queues follow these concepts:**

1. FIFO (First In First Out): This means that the first item in the queue will be the first item out of the queue. 


2. LILO (Last In Last Out): This means that the last item in the queue will be the last item out of the queue.


**Common terminology for a queue is**



1. Enqueue - Nodes or items that are added to the queue.
2. Dequeue - Nodes or items that are removed from the queue. If called when the queue is empty an exception will be raised.
3. Front - This is the front/first Node of the queue.
4. Rear - This is the rear/last Node of the queue.
5. Peek - When you peek you will view the value of the front Node in the queue. If called when the queue is empty an exception will be raised.
6. IsEmpty - returns true when queue is empty otherwise returns false.





![f](https://camo.githubusercontent.com/188c6d9e005aa95ad055a4f8a40b1d63e2084370f2b5588429d79064d289463d/68747470733a2f2f636f646566656c6c6f77732e6769746875622e696f2f636f6d6d6f6e5f637572726963756c756d2f646174615f737472756374757265735f616e645f616c676f726974686d732f436f64655f3430312f636c6173732d31302f7265736f75726365732f696d616765732f51756575652e504e47)