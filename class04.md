# Links


Links are the defining feature of the web
because they allow you to move from
one web page to another — enabling the
very idea of browsing or surfing.



**Writing Links**

Links are created using the `<a>` element. Users can click on anything
between the opening `<a>` tag and the closing `</a>` tag. You specify
which page you want to link to using the href attribute.


**Linking to Other Sites**'

Links are created using the `<a>`
element which has an attribute
called href. The value of the
href attribute is the page that
you want people to go to when
they click on the link.

**Linking to Other Pages
on the Same Site**


When you are linking to other
pages within the same site,
you do not need to specify the
domain name in the URL. You
can use a shorthand known as a
relative URL.






**Directory Structure**

On larger websites it's a good idea to organize your code by placing the
pages for each different section of the site into a new folder. Folders on a
website are sometimes referred to as directories.


**Structure**

The diagram on the right shows
the directory structure for a
fictional entertainment listings
website called ExampleArts.
The top-level folder is known
as the root folder. (In this
example, the root folder is called
examplearts.) The root folder
contains all of the other files and
folders for a website. 



**Relationships**

The relationship between
files and folders on a website
is described using the same
terminology as a family tree.

**Homepages**

The main homepage of a site
written in HTML (and the
homepages of each section in a
child folder) is called index.html


**Relative URLs**

elative URLs can be used when linking to pages within your own
website. They provide a shorthand way of telling the browser where to
find your files.


**Email Links**

To create a link that starts up
the user's email program and
addresses an email to a specified
email address, you use the `<a>`
element.

**Opening Links in a New Window**


**target**

If you want a link to open in a
new window, you can use the
target attribute on the opening
`<a>` tag. The value of this
attribute should be _blank.



**Linking to a Specific
Part of the Same Page**

At the top of a long page
you might want to add a list
of contents that links to the
corresponding sections lower
down. Or you might want to add
a link from part way down the
page back to the top of it to save
users from having to scroll back
to the top.
Before you can link to a specific
part of a page, you need to
identify the points in the page
that the link will go to. You do
this using the id attribute (which
can be used on every HTML
element). You can see that the
`<h1>` and `<h2>` elements in this
example have been given id
attributes that identify those
sections of the page.


**Linking to a Specific
Part of Another Page**


If you want to link to a specific
part of a different page (whether
on your own site or a different
website) you can use a similar
technique.


# Layout

**Key Concepts in
Positioning Elements**

**Building Blocks**

CSS treats each HTML element as if it is in its
own box. This box will either be a block-level
box or an inline box.

Block-level boxes start on a new line and act as the main building blocks
of any layout, while inline boxes flow between surrounding text. You can
control how much space each box takes up by setting the width of the
boxes (and sometimes the height, too). To separate boxes, you can use
borders, margins, padding, and background colors.

**Controlling the
Position of Elements**

CSS has the following positioning schemes that allow you to control
the layout of a page: normal flow, relative positioning, and absolute
positioning. You specify the positioning scheme using the position
property in CSS. You can also float elements using the float property.


**Normal flow**

Every block-level element
appears on a new line, causing
each item to appear lower down
the page than the previous one. 

**Relative Positioning**

This moves an element from the
position it would be in normal
flow, shifting it to the top, right,
bottom, or left of where it
would have been placed. 

**Absolute positioning**

This positions the element
in relation to its containing
element. It is taken out of
normal flow, meaning that it
does not affect the position
of any surrounding elements.

To indicate where a box should be positioned, you may also need to use
box offset properties to tell the browser how far from the top or bottom
and left or right it should be placed.

**Fixed Positioning**

This is a form of absolute
positioning that positions
the element in relation to the
browser window, as opposed
to the containing element.

Elements with fixed positioning
do not affect the position of
surrounding elements and they
do not move when the user
scrolls up or down the page.

**Floating Elements**

Floating an element allows
you to take that element out
of normal flow and position
it to the far left or right of a
containing box. The floated
element becomes a block-level
element around which other
content can flow.


**Normal Flow**

position:static

In normal flow, each block-level
element sits on top of the next
one. Since this is the default
way in which browsers treat
HTML elements, you do not
need a CSS property to indicate
that elements should appear
in normal flow, but the syntax
would be:

position: static;

position:relative

Relative positioning moves an
element in relation to where it
would have been in normal flow.

**Absolute Positioning**

position:absolute

When the position property
is given a value of absolute,
the box is taken out of normal
flow and no longer affects the
position of other elements on
the page. 

The box offset properties (top
or bottom and left or right)
specify where the element
should appear in relation to its
containing element.

**Fixed Positioning**

Fixed positioning is a type
of absolute positioning that
requires the position property
to have a value of fixed.


**Overlapping Elements**

When you use relative, fixed, or
absolute positioning, boxes can
overlap. If boxes do overlap, the
elements that appear later in the
HTML code sit on top of those
that are earlier in the page.
If you want to control which
element sits on top, you can use
the z-index property. Its value
is a number, and the higher the
number the closer that element
is to the front.


**Floating Elements**

The float property allows you
to take an element in normal
flow and place it as far to the
left or right of the containing
element as possible.

**Using Float to Place Elements Side-by-Side**

A lot of layouts place boxes
next to each other. The float
property is commonly used to
achieve this.

**Clearing Floats**

The clear property allows you
to say that no element (within
the same containing element)
should touch the left or righthand sides of a box. It can take
the following values:

left

The left-hand side of the box
should not touch any other
elements appearing in the same
containing element.

right

The right-hand side of the
box will not touch elements
appearing in the same containing
element.

both

Neither the left nor right-hand
sides of the box will touch
elements appearing in the same
containing element.

none

Elements can touch either side.

**Screen Sizes**

Different visitors to your site will have different sized screens that show
different amounts of information, so your design needs to be able to
work on a range of different sized screens.

**Screen Resolution**

Resolution refers to the number of dots a screen shows per inch. Some
devices have a higher resolution than desktop computers and most
operating systems allow users to adjust the resolution of their screens.


**Page Sizes**

Because screen sizes and display resolutions vary so much, web
designers often try to create pages of around 960-1000 pixels wide
(since most users will be able to see designs this wide on their screens).

**Fixed Width Layouts**

Fixed width layout
designs do not
change size as the
user increases
or decreases
the size of their
browser window.
Measurements tend
to be given in pixels.

**Liquid Layouts**

Liquid layout designs
stretch and contract
as the user increases
or decreases the
size of their browser
window. They tend to
use percentages.


**CSS Frameworks**

CSS frameworks aim to make your life easier by providing the code for
common tasks, such as creating layout grids, styling forms, creating
printer-friendly versions of pages and so on. You can include the CSS
framework code in your projects rather than writing the CSS from scratch.

# Functions, Methods, and Objects 

Browsers require very detailed instructions about what
we want them to do. Therefore, complex scripts can run
to hundreds (even thousands) of lines. Programmers use
functions, methods, and objects to organize their code. 


 **what is the function?**

a function allows you to define a block of code, give it a name and then execute it as many times as you want. 

 **declaring a function**
You can declare a function by providing its return value, name, and the types for its arguments. 

function functionName (argument1,argument2,....)

{
    statements;
}

**Invoking afunction**

functions are called by specifying the name of the function, followed by the parentheses. The parentheses may or may not contain a list of arguments depending on the function definition.

functionName();

# pair programming

Iterative loops. Code reviews. Fast feedback. Error checking and linting. These are software engineering practices that have proven to dramatically improve the quality of code developers produce. What if you can could get all of this, instantaneously, while typing code line by line and character by character? You can, with pair programming, a technique common to many agile work environments.

**How does pair programming work?**

Pair programming is an agile software development technique in which two programmers work together at one workstation. One, the driver, writes code while the other, the observer or navigator,reviews each line of code as it is typed in.


**Why pair program?**
1. Greater efficiency
2. Engaged collaboration
3. Learning from fellow students
4. Social skills
5. Job interview readiness
6. Work environment readiness








