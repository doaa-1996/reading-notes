# Objects

**WHAT IS AN OBJECT?** 

Objects group together a set of variables and functions to create a model
of a something you would recognize from the real world. In an object,
variables and functions take on new names. 


If a variable is part of an object, it is called a
property. Properties tell us about the object, such as
the name of a hotel or the number of rooms it has.
Each individual hotel might have a different name
and a different number of rooms. 


If a function is part of an object, it is called a method.
Methods represent tasks that are associated with
the object. For example, you can check how many
rooms are available by subtracting the number of
booked rooms from the total number of rooms.



Like variables and named functions,
properties and methods have a
name and a value. In an object,
that name is called a key.


An object cannot have two keys
with the same name. This is
because keys are used to access
their corresponding values. 


The value of a property can be a
string, number, Boolean, array, or
even another object. The value of a
method is always a function. 


The object literal is a simple way of creating an object using { } brackets. You can include key-value pair in { }, where key would be property or method name and value will be value of property of any data type or a function. Use comma (,) to separate multiple key-value pairs.



`var <object-name> = { key1: value1, key2: value2,... keyN: valueN};`


**Accessing an object in JS**


To access a property of this
object, the object name is
followed by a dot (the period
symbol) and the name of the
property that you want.


`objectName.propertyName`



# The Document Object Model



![dom](https://www.w3schools.com/js/pic_htmltree.gif)





* As a browser loads a web page, it creates a model of that page.
The model is called a DOM tree, and it is stored in the browsers' memory.
It consists of four main types of nodes.
* Each node is an object with methods and properties.
Scripts access and update this DOM tree (not the source HTML file).
Any changes made to the DOM tree are reflected in the browser.
 1. THE DOCUMENT NODE (html , head , body ,...)
 2. ELEMENT NODES (h1 , p, ..)
 3. ATTRIBUTE NODES (div , script , li)
 4. TEXT NODES
**Accessing and updating the DOM tree involves two steps:**
1. Locate the node that represents the element you want to work with.
2. Use its text content, child elements, and attributes.
1. **STEP 1: ACCESS THE ELEMENTS**
   * SELECT AN INDIVIDUAL ELEMENT NODE
   * SELECT MULTIPLE ELEMENTS (NODELISTS)
   * TRAVERSING BETWEEN ELEMENT NODES
2. **STEP 2: WORK W ITH THOSE ELEMENTS**
   * ACCESS/ UPDATE TEXT NODES
   * WORK W ITH HTML CONTENT
   * ACCESS OR UPDATE ATTRIBUTE VALUES
**CACHING DOM QUERIES**
* Methods that find elements in the DOM tree are called DOM queries. When you need to work with an element more than once, you should use a variable to store the result of this query.
* When a script selects an element to access or update, the Interpreter must find the elementca) in the DOM tree.
**ACCESSING ELEMENTS**
* DOM queries may return one element, or they may return a Nodelist,
which is a collection of nodes.
* GROUPS OF ELEMENT NODES
If a method can return more than one node, it will
always return a Nodelist, which is a collection of
nodes
* FASTEST ROUTE
Finding the quickest way to access an element
within your web page will make the page seem
faster and/or more responsive.
* METHODS THAT RETURN A SINGLE ELEMENT NODE:
1. getElementByld :
Selects an individual element given the value of its i d attribute .
The HTML must have an id attribute in order for it to be selectable.
2. querySel ector
Uses CSS selector syntax that would select one or more elements .
This method returns only the first of the matching elements
  **METHODS THAT RETURN ONE OR MORE ELEMENTS (AS A NODELIST):**
  1. getEl ementsByClassName( 1
class 1 )
Selects one or more elements given the value of their cl ass attribute.
The HTML must have a cl ass attribute for it to be selectable.
This method is faster than querySe 1ectorA11 () .
2. getEl ementsByTagName
Selects all elements on the page with the specified tag name.
This method is faster than querySe 1ectorA11 ().
3. querySelectorAll
Uses CSS selector syntax to select one or more elements and returns all
of those that match.
**TRAVERSING THE DOM**
* When you have an element node, you can select
another element in relation to it using these five
properties. This is known as traversing the DOM.
1. parentNode
This property finds the element
node for the containing (or
parent) element in the HTML
2. previousSibling
nextSibling
These properties find the
previous or next sibling of a node
if there are siblings.
3. first Child-lastChild
These properties find the first or
last child of the current element.
**WHITESPACE NODES**
Traversing the DOM can be difficult because
some browsers add a text node whenever they
come across whitespace between elements
**HOW TO GET/UPDATE ELEMENT CONTENT**
* When you select a text node, you can retrieve or amend the content of it
using the node Va 1 ue property.
ex :
document.getElementByid( 1 one 1 ).firstChild.nextSibling. nodeValue;
* get El ementByi d () allows you
to select a single element node
by specifying the value of its
id attribute.
This method has one parameter:
the value of the id attribute on
the element you want to select.
**When a DOM query returns a Nodelist, you may want to:**
1. Select one element from the NodeList.
2. Loop through each item in the Nodelist and
perform the same statements on each of the
element nodes.
* In a **live Nodelist**, when your script updates the
page, the Nodelist is updated at the same time.
The methods beginning getEl ementsBy_ return live
Node lists. They are also typically faster to generate
than static Nodelists.
* In a **static Nodelist** when your script updates the
page, the NodeList is not updated to reflect the
changes made by the script.
*ACCESSING TEXT ONLY*
* The script starts off by getting
the content of the first list item
using both the textContent
**ADDING OR REMOVING HTML CONTENT**
  * There are two very different approaches to adding and removing content from a DOM tree: the innerHTML property and DOM manipulation.
1. APPROACH :
   Inner can be used on any element node. It is used both to retrieve and replace content. To update an element, new content is provided as a string It can contain markup for descendant elements.
2. ADDING :
   CONTENT To add new content 1. Store new content (including markup) asa string in a variable. 2. Select the element whose content you want to replace. 3. Set the element's InnerHTHL property to be the new string
3. REMOVING :
  CONTENT To remove all content from an element, you set innerNTML to an empty string To remove one element from a DOM fragment, eg, one <11> from a ul, you need to provide the entire fragment minus that element.
* document.write()
* The document object's write () method is a simple
way to add content that was not in the original
source code to the page, but its use is rarely advised.
**ADVANTAGES**
1. It is a quick and easy way to show beginners how content can be added to a page.
**DISADVANTAGES**
1. It only works when the page initially loads.
2. If you use it after the page has loaded it can:
3. Overwrite the whole page
4. Not add the content to the page
5. Create a new page
6. It can cause problems with XHTML pages that
are strictly validated.
7. This method is very rarely used by programmers
these days and is generally frowned upon.
**CREATING ATTRIBUTES & CHANGING THEIR VALUES**
* The className property allows
you to change the value of the
class attribute. If the attribute
does not exist, it will be created
and given the specified value.
cOS/js/set-attribute.js
You have seen this property
used throughout the chapter
to update the status of the
list items. Below, you can see
another way to achieve the task.
The setAttri bute() method
allows you to update the value
of any attribute. It takes two
parameters: the attribute name,
and the value for the attribute.
**REMOVING ATTRI BUTES**
To remove an attribute from an
element, first select the element,
then call removeAtt r i bute () .
It has one parameter: the name
of the attribute to remove.














