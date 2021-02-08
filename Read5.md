# Comparison and Logical Operators

  **Comparison operators** allow you to compare two values,determine equality or difference between variables or values.

  These are some comparison operators:

* ==	equal to.

* ===	equal value and equal type.

* !=	not equal.

* !==	not equal value or not equal type.

* 	greater than.


* <	less than.

* >= greater than or equal to.

* <=	less than or equal to.




**Logical Operators** are used to determine the logic between variables or values such as :



 ## &&	and
 
 The logical AND operator (&&) returns true if both operands are true and returns false otherwise.


##  ||	or
The logical OR ( || ) operator (logical disjunction) for a set of operands is true if and only if one or more of its operands is true.


 ## !	not
 eturns TRUE or 1 when the operand is FALSE or 0, and returns FALSE or 0 when the operand is TRUE or 1.


 # loops

 Loops are used in JavaScript to perform repeated tasks based on a condition. Conditions typically return true or false when analysed. A loop will continue running until the defined condition returns false .

 **The three most common types of loops are:**

for
while
do while

we will talk about for and while loops:

## for loop

*for ([initialization]); [condition]; [final-expression])


 {
   // statement
}*

## Description

**initialization** - Run before the first execution on the loop. This expression is commonly used to create counters. Variables created here are scoped to the loop. Once the loop has finished it’s execution they are destroyed.

**condition** - Expression that is checked prior to the execution of every iteration. If omitted, this expression evaluates to true. If it evaluates to true, the loop’s statement is executed. If it evaluates to false, the loop stops.

**final-expression** - Expression that is run after every iteration. Usually used to increment a counter. But it can be used to decrement a counter too.

**statement** - Code to be repeated in the loop.



## While loop

while (condition)

{

  statement(s);

}

## Description


**statement(s):** A statement that is executed as long as the condition evaluates to true.

**condition:** Here, condition is a Boolean expression which is evaluated before each pass through the loop. If this condition evaluates to true, statement(s) is/are executed. When condition evaluates to false, execution continues with the statement after the while loop.



