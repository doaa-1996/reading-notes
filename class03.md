 
 **Lists**

HTML provides us with three different types:

**Ordered lists** are lists where each item in the list is numbered.

The ordered list is created with the `<ol>` element.

Each item in the list is placed between an opening `<li>` tag and a closing `</li>` tag.


**Unordered lists** are lists that begin with a bullet point.

The unordered list is created with the `<ul>` element.

Each item in the list is placed between an opening `<li>` tag and a closing `</li>` tag.



**Definition lists** are made up of a set of terms along with the definitions for each of those terms.

The definition list is created with the `<dl>` element and usually consists of a series of terms and their definitions.

Inside the `<dl>` element you will usually see pairs of `<dt>` and `<dd>` elements.

`<dt>`
This is used to contain the term being defined (the definition term).

`<dd>`
This is used to contain the definition.


**Nested Lists**

You can put a second list inside an `<li>` element to create a sublist or nested list.


## Boxes

You can set several properties that affect the appearance of these boxes.

CSS treats each HTML element as if it lives in its own box.

**Box Dimensions**


The most popular ways to specify the size of a box are to use pixels, percentages, or
ems.

**Limiting Width**
min-width, max-width

Some page designs expand and shrink to fit the size of the user's screen. In such designs, the min-width property specifies
the smallest size a box can be displayed at when the browser window is narrow, and the max-width property indicates the maximum width a box can stretch to when the browser window is wide.

**Limiting Height**
min-height, max-height

n the same way that you might want to limit the width of a box on a page, you may also want to limit the height of it. This is achieved using the min-height and max-height properties.

**Overflowing Content**

The overflow property tells the browser what to do if the content contained within a box is larger than the box itself. 

It can have one of two values:

**hidden**

This property simply hides any extra content that does not fit in the box.

**scroll**

This property adds a scrollbar to the box so that users can scroll to see the missing content.

**Border, Margin & Padding**

**Border**

Every box has a border (even if it is not visible or is specified to be 0 pixels wide). The border separates the edge of one box from another.

**Margin**

Margins sit outside the edge of the border. You can set the width of a margin to create a gap between the borders of two
adjacent boxes.

**Padding**

Padding is the space between the border of a box and any content contained within it.
Adding padding can increase the readability of its contents.

**Border Width**

The border-width property is used to control the width of a border. The value of this property can either be given in pixels or using one of the following values:

thin

medium

thick

**Border Style**

You can control the style of a
border using the border-style
property. This property can take
the following values:

solid: a single solid line.

dotted: a series of square dots
(if your border is 2px wide, then
the dots are 2px squared with a
2px gap between each dot).

dashed: a series of short lines.

double: two solid lines (the
value of the border-width
property creates the sum of the
two lines).

groove: appears to be carved
into the page.

ridge: appears to stick out from
the page.

inset: appears embedded into
the page.

outset: looks like it is coming
out of the screen.

hidden / none: no border is
shown.

You can individually change the
styles of different borders using:

border-top-style
border-left-style
border-right-style
border-bottom-style

**Border Color**

You can specify the color of a
border using either RGB values,
hex codes or CSS color names 

It is possible to individually
control the colors of the borders
on different sides of a box using:

border-top-color
border-right-color
border-bottom-color
border-left-color

It is also possible to use a
shorthand to control all four
border colors in the one
property:


border-color: darkcyan

deeppink darkcyan

deeppink;



**Shorthand
border**

The border property allows you
to specify the width, style and
color of a border in one property
(and the values should be coded
in that specific order).


**Padding**

The padding property allows
you to specify how much space
should appear between the
content of an element and its
border. 

You can specify different values
for each side of a box using:

padding-top

padding-right

padding-bottom

padding-left


**Margin**

The margin property controls
the gap between boxes. Its value
is commonly given in pixels,
although you may also use
percentages or ems.

You can specify values for each
side of a box using:

margin-top

margin-right

margin-bottom

margin-left

**Centering Content**

If you want to center a box on
the page (or center it inside
the element that it sits in), you
can set the left-margin and
right-margin to auto.

In order to center a box on the
page, you need to set a width
for the box (otherwise it will take
up the full width of the page).

**display**
The display property allows
you to turn an inline element
into a block-level element or vice
versa, and can also be used to
hide an element from the page.

The values this property can
take are:

inline

This causes a block-level
element to act like an inline
element.
block

This causes an inline element to
act like a block-level element.

inline-block

This causes a block-level
element to flow like an inline
element, while retaining other
features of a block-level element.

none

This hides an element from the
page.

**border-image**

The border-image property
applies an image to the border of
any box. It takes a background
image and slices it into nine
pieces. 

**box-shadow**

he box-shadow property
allows you to add a drop shadow
around a box. 

 It must
use at least the first of these two
values as well as a color:

Horizontal offset

Negative values position the
shadow to the left of the box.

Vertical offset

Negative values position the
shadow to the top of the box.

Blur distance

If omitted, the shadow is a solid
line like a border.

Spread of shadow

If used, a positive value will
cause the shadow to expand in
all directions, and a negative
value will make it contract.

**border-radius**

CSS3 introduces the ability to
create rounded corners on any
box, using a property called
border-radius. The value
indicates the size of the radius
in pixels.

# Javascript

An array is a special type of variable. It doesn't
just store one value; it stores a list of values. 

CREATING AN ARRAY 

You create an array and give it
a name just like you would any
other variable (using the var
keyword followed by the name of
the array).

The values are assigned to the
array inside a pair of square
brackets, and each value is
separated by a comma.

Values in an array are accessed as if they are in
a numbered list. It is important to know that the
numbering of this list starts at zero (not one). 

**SWITCH STATEMENTS** 

A switch statement starts with a
variable called the switch value.
Each case indicates a possible
value for this variable and the
code that should run if the
variable matches that value. 

**loops**



Looping in programming languages facilitates the execution of a set of instructions/functions repeatedly while some condition evaluates to true.

Following are the types of loops in JavaScript:

1) while loop
2) for loop
3) do-while

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


The do...while statement repeats until a specified condition evaluates to false.

**Syntax**

do

  statement
  
while (condition);






















