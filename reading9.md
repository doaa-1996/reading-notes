# Concepts of Functional Programming in Javascript

## What is functional programming?

Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data.


we used to use Object-Oriented Programming in most of our real-world use-cases for better or for worse. Most use-cases of Functional Programming back then rely solely on mathematical computations whether simple or complex and the usage of it in components like buttons, textbox, checkbox never really fit in most of our scenarios.




## Features of Functional Programming


***1. First-Class Citizen Functions***

What’s good about Functional Programming is its functions are first-class citizens: you can always insert functions inside a function without any restrictions present.

function executeFunctions(x, y) {
    const add = (x, y) => x + y;
    const subtract = (x, y) => x — y;
    console.log(`sum: ${add(x,y)}`);
    console.log(`difference: ${subtract(x,y)}`);
}



***2. Higher-Order Functions***

A higher-order function is a function that gets a function as an argument. It may or may not return a function as its resulting output.

function greaterThan(n) {
return x => x > n;
}
let greaterThanTwo = greaterThan(2);
console.log(greaterThanTwo(5));



***3. Function Composition***

Functional Programming won’t be completely functional without this feature. Function Composition is an act of composing/creating functions that allow you to further simplify and compress your functions by taking functions as an argument and return an output. It may also return another function as its output other than numerical/string values.



***Benefits of Functional Programming***

1. It doesn’t have side-effects and it’s immutable
2. It’s clean, straightforward, succinct




# Refactoring JavaScript for Performance and Readability 


Think of refactoring your code as re-writing it so that it’s easier to read and easier to work with in the future.


The Basics of Refactoring Your Code

To refactor your code, you can basically go through a fairly simple 3 step process. If you implement this into your coding habits, you will notice fairly quickly that your code will start to look much more professional and tidy. The image below shows the typical 3 step process that you should go through when refactoring your code.


![img](https://camo.githubusercontent.com/0d61eedfe52646223c8080350c5cf02168d519498bc74ac0d7bd44d88bc053fa/68747470733a2f2f63646e2d696d616765732d312e6d656469756d2e636f6d2f6d61782f313032342f312a6e4358366273534e55465f763268464b676e615149412e706e67)