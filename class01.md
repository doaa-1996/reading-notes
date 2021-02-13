 # ***Web Design Overview***

 The web design process starts with a visual concept, which you could sketch by hand or with software like Photoshop. Then, you use HTML and CSS to build the website. HTML and CSS are the codes for writing web pages. HTML handles the basic structure and ‘bones’ of your page, while CSS handles the style and appearance.


HTML Uses Elements to Describe the Structure of Pages
There are several different elements, Each element has an opening tag and a closing tag.

Tags act like containers. They tell you something about the information that lies between their opening and closing tags.


Attributes provide additional information
about the contents of an element. They appear
on the opening tag of the element and are
made up of two parts: a name and a value,
separated by an equals sign.

each HTML structure contains two parts: a head and a body

The head contains information about the page (rather than information that is shown within the main part of the browser window that is highlighted in blue on the opposite page). 

Everything inside the body is shown inside the main browser window.


Because there have been several versions of HTML, each web page should begin with a DOCTYPE declaration to tell a browser which version of HTML the page is using (although browsers usually display the page even if it is not included). 

If you want to add a comment to your code that will not be visible in the user's browser, you can add the text between these characters:

![HTML comment](https://www.copahost.com/blog/wp-content/uploads/2019/07/html-comments.jpg)


ID Attribute
Every HTML element can carry the id attribute. It is used to uniquely identify that element from other elements on the page.

Class Attribute
Its value should describe the class it belongs to.

Block Elements
Some elements will always appear to start on a new line in the browser window. These are known as block level elements.

Inline Elements
Some elements will always appear to continue on the
same line as their neighbouring elements. These are known as inline elements.

Grouping Text & Elements In a Block
The div element allows you to group a set of elements together in one block-level box.

Grouping Text & Elements Inline The span element acts like an inline equivalent of the div
element. 
It is used to either:

1. Contain a section of text
where there is no other suitable
element to differentiate it from
its surrounding text.
2. Contain a number of inline
elements.

IFrames
An iframe is like a little window that has been cut into your page — and in that window you
can see another page.

There are a few attributes that you will need
to know to use it:

* src The src attribute specifies the
URL of the page to show in the frame.

* height The height attribute specifies
the height of the iframe in pixels.

* width
The width attribute specifies the width of the iframe in pixels.

scrolling
The scrolling attribute will not be supported in HTML5. In HTML 4 and XHTML, it indicates whether the iframe should have scrollbars or not. This is important if the page inside the iframe is larger than the space you have allowed for it (using the
height and width attributes). Scrollbars allow the user to move around the frame to see more content. It can take one of three values: yes (to show scrollbars), no (to hide scrollbars) and auto
(to show them only if needed).

frameborder
The frameborder attribute will not be supported in HTML5. In HTML 4 and XHTML, it indicates whether the frame should have a border or not. A value of 0 indicates that no border should be shown. A value of 1 indicates that a border should be shown.

seamless
In HTML5, a new attribute called seamless can be applied to an iframe where scrollbars are not desired. The seamless attribute (like some other new
HTML5 attributes) does not need a value, but you will often see authors give it a value of seamless. Older browsers do not support the seamless attribute.

The meta element lives inside the head element and contains information about that web page.
It is not visible to users but fulfills a number of purposes such as telling search engines about your page, who created it, and whether or not it is time
sensitive. (If the page is time sensitive, it can be set to expire.)
The meta element is an empty element so it does not have a closing tag. It uses attributes to
carry the information.


HTML5 introduces a new set of elements that allow you to divide up the parts of a page. The names of these elements indicate the kind of content you will find in them.

 The header and footer elements can be used for:

● The main header or footer that appears at the top or bottom of every page on the site.
● A header or footer for an individual article or
section within the page.


The nav element is used to contain the major navigational blocks on the site such as the primary site navigation.

The article element acts as a container for any section of a page that could stand alone and
potentially be syndicated.

The purpose of the hgroup element is to group together a set of one or more h1 through h6 elements so that they are treated as one single heading.


Site Maps

The aim is to create a diagram of the pages that will be used to structure the site. This is known as a site map and it will show how those pages can be
grouped.

WireFrames

A wireframe is a simple sketch of the key information that needs to go on each page of a site. It shows the hierarchy of the information and how much space it might require.

we use javascript to make the web page interactive and dynamic.

A script is a series of instructions that a
computer can follow to achieve a goal. 

To approach writing a script, break down your goal into a series of tasks and then work out each step needed to complete that task (a flowchart can help). 

