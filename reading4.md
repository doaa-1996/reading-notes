 ***Grids in CSS:***

 The CSS Grid Layout Module offers a grid-based layout system, with rows and columns, making it easier to design web pages without having to use floats and positioning.

A grid layout consists of a parent element, with one or more child elements. An HTML element becomes a grid container when its display property is set to grid or inline-grid.


All direct children of the grid container automatically become grid items. The vertical lines of grid items are called columns. The horizontal lines of grid items are called rows. The spaces between each column/row are called gaps.


You can adjust the gap size by using one of the following properties:

grid-column-gap: sets the gap between the columns.

grid-row-gap: sets the gap between the rows.

grid-gap: is a shorthand property for the grid-row-gap and the grid-column-gap properties.



The lines between columns are called column lines.

The lines between rows are called row lines. Refer to line numbers when placing a grid item in a grid container:


***RegEx:***

A regular expression is an object that describes a pattern of characters. Regular expressions are used to perform pattern-matching and "search-and-replace" functions on text.

Syntax: /pattern/modifiers;


Modifiers are used to perform case-insensitive and global searches: g Perform a global match (find all matches rather than stopping after the first match). i Perform case-insensitive matching. m Perform multiline matching.


- Brackets are used to find a range of characters:


[abc] Find any character between the brackets.

[^abc] Find any character NOT between the brackets.

[0-9] Find any character between the brackets (any digit).

[^0-9] Find any character NOT between the brackets (any non-digit).

(x|y) Find any of the alternatives specified.



RegExp Object Properties

constructor Returns the function that created the RegExp object's prototype. global Checks whether the "g" modifier is set. ignoreCase Checks whether the "i" modifier is set. lastIndex Specifies the index at which to start the next match. multiline Checks whether the "m" modifier is set. source Returns the text of the RegExp pattern.



RegExp Object Methods:


compile() Deprecated in version 1.5. Compiles a regular expression.

exec() Tests for a match in a string. Returns the first match.

test() Tests for a match in a string. Returns true or false.

toString() Returns the string value of the regular expression.



Responsice Web Design (RWD):

Responsive web design is the practice of building a website suitable to work on every device and every screen size, no matter how large or small, mobile or desktop.


Currently the most popular technique lies within responsive web design, favoring design that dynamically adapts to different browser and device viewports, changing layout and content along the way. This solution has the benefits of being all three, responsive, adaptive, and mobile.


Responsive generally means to react quickly and positively to any change, while adaptive means to be easily modified for a new purpose or situation, such as change.