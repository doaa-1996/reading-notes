# Domain Modeling

Domain modeling is the process of creating a conceptual model in code for a specific problem. A model describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain. An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an object-oriented model.

A domain model that's articulated well can verify and validate the understanding of a specific problem among various stakeholders. As a communication tool, it defines a vocabulary that can be used within and between both technical and business teams.



Define a constructor and initialize properties

To define the same properties between many objects, you'll want to use a constructor function. Below is a table that summarizes a JavaScript representation of an EpicFailVideo object.

 

Type
|Property     | Data        |   Type  |
| ------------|-------------|---------|
 epicRating   |1 to 10      | Number  |
|hasAnimals   |true or fals |Boolean  |





Domain modeling is the process of creating a conceptual model for a specific problem. And a domain model that's articulated well can verify and validate your understanding of that problem.


Here's some tips to follow when building your own domain models.


When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors.

Model its attributes with a constructor function that defines and initializes properties.

Model its behaviors with small methods that focus on doing one job well.

Create instances using the new keyword followed by a call to a constructor function.

Store the newly created object in a variable so you can access its properties and methods from outside.

Use the this variable within methods so you can access the object's properties and methods from inside.


# Tables

There are several types of information
that need to be displayed in a grid or
table. For example: sports results, stock
reports, train timetables.


**What's a Table?**

A table represents information in a grid format.
Examples of tables include financial reports, TV
schedules, and sports results.

**Basic Table Structure**


<table>

The `<table>` element is used
to create a table. The contents
of the table are written out row
by row.


`<tr>`

You indicate the start of each
row using the opening `<tr>` tag.
(The tr stands for table row.)
It is followed by one or more
<`td>` elements (one for each cell
in that row).

At the end of the row you use a
closing `</tr>` tag.

`<td>`

Each cell of a table is
represented using a `<td>`
element. (The td stands for
table data.)
At the end of each cell you use a
closing `</td>` tag.



**Table Headings**

`<th>`

The `<th>` element is used just
like the `<td>` element but its
purpose is to represent the
heading for either a column or
a row. (The th stands for table
heading.) 


**Spanning Columns**

The colspan attribute can be
used on a `<th>` or `<td>` element
and indicates how many columns
that cell should run across.


**Spanning Rows**

The rowspan attribute can be
used on a `<th>` or `<td>` element
to indicate how many rows a cell
should span down the table.


**Long Tables**

There are three elements that
help distinguish between the
main content of the table and
the first and last rows (which can
contain different content).
These elements help people
who use screen readers and also
allow you to style these sections
in a different manner than the
rest of the table (as you will see
when you learn about CSS).


`<thead>` 

The headings of the table should
sit inside the `<thead>` element.

`<tbody>`

The body should sit inside the
`<tbody>` element.

`<tfoot>`

The footer belongs inside the
`<tfoot>` element.



**Old Code:
Width & Spacing**

There are some outdated
attributes which you should not
use on new websites. You may,
however, come across some
of them when looking at older
code, so I will mention them
here. All of these attributes have
been replaced by the use of CSS.

The width attribute was used
on the opening `<table>` tag to
indicate how wide that table
should be and on some opening
`<th>` and `<td>` tags to specify
the width of individual cells.
The value of this attribute is
the width of the table or cell in
pixels.

The columns in a table need to
form a straight line, so you often
only see the width attribute on
the first row (and all subsequent
rows would use that setting).

The opening `<table>` tag could
also use the cellpadding
attribute to add space inside
each cell of the table, and the
cellspacing attribute to create
space between each cell of
the table. The values for these
attributes were given in pixels.



**Old Code:
Border & Background**

The border attribute was used
on both the `<table>` and `<td>`
elements to indicate the width of
the border in pixels.
The bgcolor attribute was used
to indicate background colors
of either the entire table or
individual table cells. The value
is usually a hex code.



# Functions, Methods, and Objects

 # Functions

## what is the function?

a function allows you to define a block of code, give it a name and then execute it as many times as you want. 

## declaring a function
You can declare a function by providing its return value, name, and the types for its arguments. 

*function functionName (argument1,argument2,....)*

*{
    statements;
}*

## Invoking afunction

functions are called by specifying the name of the function, followed by the parentheses. The parentheses may or may not contain a list of arguments depending on the function definition.

*functionName();*



## Methods

JavaScript methods are actions that can be performed on objects.

A JavaScript method is a property containing a function definition.


You access an object method with the following syntax:

`objectName.methodName()`

You will typically describe fullName() as a method of the person object, and fullName as a property.

The fullName property will execute (as a function) when it is invoked with ().

## Object
An object is a collection of properties, and a property is an association between a name (or key) and a value. 


The object literal is a simple way of creating an object using { } brackets. You can include key-value pair in { }, where key would be property or method name and value will be value of property of any data type or a function. Use comma (,) to separate multiple key-value pairs.



`var <object-name> = { key1: value1, key2: value2,... keyN: valueN};`


**Accessing an object in JS**


To access a property of this
object, the object name is
followed by a dot (the period
symbol) and the name of the
property that you want.


`objectName.propertyName`
