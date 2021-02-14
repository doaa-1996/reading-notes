 # ***Web design overview***

 ## ***Mark up***

When creating a web page, you add tags (known as markup) to the contents of the page. These tags provide extra meaning and allow browsers to show users the appropriate structure for the page.

How to add markup to the text that
appears on your page?

There are two types of markup: 

## ***Structural markup***


***Headings***

HTML has six "levels" of headings:
h1 is used for main headings
h2 is used for subheadings 
If there are further sections under the subheadings then the h3 element is used, and so on...


***Paragraphs***

To create a paragraph, surround the words that make up the paragraph with an opening p tag and closing /p tag.

***Bold & Italic***

By enclosing words in the tags b and /b we can make characters appear bold.

By enclosing words in the tags  i and /i we can make characters appear italic.

***Superscript & Subscrip***

The sup element is used to contain characters that should be superscript such as the suffixes of dates or mathematical concepts like raising a number to a power such as 22 .

The sub element is used to contain characters that should
be subscript. It is commonly used with foot notes or chemical formulas such as H20.

Line Breaks & Horizontal Rules

if you wanted to add a line break inside the middle of a paragraph you can use the line break tag br /

To create a break between themes — such as a change of
topic in a book or a new scene in a play — you can add a
horizontal rule between sections using the hr / tag.

## ***Semantics marrkup***

There are some text elements that are not intended to affect the structure of your web pages, but they do add extra information to the pages — they are known as semantic markup.

***Strong & Emphasis***

The use of the strong element indicates that its content has strong importance.

The em element indicates emphasis that subtly changes the meaning of a sentence.

***Quotations***

There are two elements commonly used for marking up
quotations:

The blockquote element is used for longer quotes that take
up an entire paragraph. 

The q element is used for shorter quotes that sit within
a paragraph. 


***Abbreviations & Acronyms***

If you use an abbreviation or an acronym, then the abbr
element can be used. A title attribute on the opening tag is
used to specify the full term.

In HTML 4 there was a separate acronym element for
acronyms. To spell out the full form of the acronym, the titleattribute was used (as with the abbr elem
ent above). HTML5 just uses the abbtir element for both abbreviaons and acronyms.


***Citations & Definitions***

When you are referencing a piece of work such as a book,
film or research paper, the cite element can be used
to indicate where the citation is from.

The first time you explain some new terminology (perhaps an
academic concept or some jargon) in a document, it is
known as the defining instance of it.

The dfn element is used to indicate the defining instance of
a new term.

***Author Details***

The address element has quite a specific use: to contain
contact details for the author of the page.


***Changes to Content***

The ins element can be used to show content that has been
inserted into a document, while the del element can show text that has been deleted from it.


The s element indicates something that is no longer
accurate or relevant (but that should not be deleted).


## ***Introducing CSS***

In this section, we will look at how to make your web pages more attractive, controlling the design of them using CSS.

CSS treats each HTML element as if it appears inside
its own box and uses rules to indicate how that
element should look.

CSS declarations sit inside curly brackets and each is made up of two parts: a property and a value, separated by a colon. You can specify several properties in one declaration, each separated by a semi-colon.

***Using External CSS***

The link element can be used in an HTML document to tell the browser where to find the CSS file used to style the page.

href
This specifies the path to the CSS file (which is often placed in a folder called css or styles).

type
This attribute specifies the type of document being linked to. The value should be text/css.

rel
This specifies the relationship between the HTML page and the file it is linked to. The value should be stylesheet when linking to a CSS file.

***Using Internal CSS***

You can also include CSS rules within an HTML page by placing them inside a style element, which usually sits inside the head element of the page. 

***CSS Selectors***

There are many different types of CSS selector that allow you to target rules to specific elements in an HTML document.


## ***Javascript***

A script is a series of instructions that a computer can follow one-by-one.
Each individual instruction or step is known as a statement.
Statements should end with a semicolon. 

***COMMENTS***

You should write comments to explain what your code does.
They help make your code easier to read and understand.
This can help you and others who read your code. 


To write a comment that stretches over more than
one line, you use a multi-line comment, starting with the /* characters and ending with the */ characters.

In a single-line comment, anything that follows the
two forward slash characters I/ on that line will not be processed by the JavaScript interpreter.

**WHAT IS A VARIABLE?**

A script will have to temporarily store the bits of information it needs to do its job. It can store this data in variables.

You declare a JavaScript variable with the var keyword:

var varName;

After the declaration, the variable has no value (technically it has the value of undefined).

To assign a value to the variable, use the equal sign:

varName = value;

***DATA TYPES***

JavaScript distinguishes between numbers, strings, and true or false values known as Booleans.

***ARRAYS***

An array is a special type of variable. It doesn't
just store one value; it stores a list of values. 

***CREATING AN ARRAY*** 

You create an array and give it a name just like you would any other variable (using the var keyword followed by the name of the array). The values are assigned to the array inside a pair of square brackets, and each value is separated by a comma.

Values in an array are accessed as if they are in
a numbered list. It is important to know that the
numbering of this list starts at zero (not one). 


***EXPRESSIONS***

An expression evaluates into (results in) a single value. Broadly speaking there are two types of expressions. 

***OPERATORS***

Expressions rely on things called operators; they allow programmers to create a single value from one or more values.

***ARITHMETI C OPERATORS***

JavaScript contains the following mathematical operators, which you can use with numbers. 

![Arithmatic operators](https://contribute.geeksforgeeks.org/wp-content/uploads/arithmetic-operators.png)


***STRING OPERATOR*** 

There is just one string operator: the+ symbol.
It is used to join the strings on either side of it. 

***Decisions and loops***

A programming language uses control statements to control the flow of execution of the program based on certain conditions.

Comparison operators are used in logical statements to determine equality or difference between variables or values.

Comparison operators can be used in conditional statements to compare values and take action depending on the result.


![](https://www.pylenin.com/img/comparison-operators/comparison-table-2.png)


Logical operators are used to determine the logic between variables or values.

![](https://i.ytimg.com/vi/JVL6xEzOCrE/maxresdefault.jpg)





JavaScript’s conditional statements are:

1) if
2) if-else


 ***if statement***

if statement is the most simple decision making statement.

It is used to decide whether a certain statement or block of statements will be executed or not.

If a certain condition is true then a block of statement is executed otherwise not.

**Syntax**

if ( condition ) 

{
   // block of code to be executed
}

 ***if…else statement***

 The if-else statement has two parts if block and else block.

If the condition is true then if block (true block) will get executed and if the condition is false then else block (false block) will get executed.

**Syntax**

if ( condition )  

{
    // block of code to be executed when condition is true
} 

else 
{
    // block of code to be executed when condition is false
}


***Looping Statements***

Looping in programming languages facilitates the execution of a set of instructions/functions repeatedly while some condition evaluates to true.

Following are the types of loops in JavaScript:

1) while loop
3) for loop

A while loop is a entry-controlled loop that allows code to be executed repeatedly if the condition is true.

When the condition becomes false, the loop terminates which marks the end of its life cycle.

**Syntax**

while (condition)

{
   // Statements to be executed
}

A for loop is a entry-controlled loop that allows code to be executed repeatedly.

Unlike a while loop, a for statement consumes the initialization, condition and increment/decrement in one line thereby providing a shorter, easy to debug structure of looping.


**Syntax**

for (initialization; condition; increment/decrement)

{
    // Statements to be executed
}














