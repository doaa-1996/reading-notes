# JQuery

jQuery offers a simple way to achieve a variety of common JavaScript tasks quickly and consistently, across all major browsers and without any fallback code needed.


WHAT IS JQUERY? jQuery is a JavaScript file that you include in your webpages it lets find elements using CSS-style selectors and then do something with the elements using jQuery methods.


1. find elements using CSS-style selectors
example: $(‘Selectos’)
2. do something with the elements using jQuery methods example: $(‘li.hot’).addClass(‘complete)

WHY USE JQUERY? jQuery doesn’t do anything you cannot achieve with pure JavaScript. It is just a JavaScript file but estimates show it has been used on over a quarter of the sites on the web, because it makes coding simpler.


***SIMPLE SELECTORS***

 As you saw in Chapter 5, which introduced the DOM, it is not always easy to select the elements that you want to. For example: • Older browsers do not support the latest methods for selecting elements. • IE does not treat whitespace between elements as text nodes, while other browsers do. Such issues make it hard to select the right elements on a page across all major browsers. Rather than learn a new way to select elements, jQuery uses a language that is already familiar to front-end web developers: CSS selectors. They: • Are much faster at selecting elements • Can be a lot more accurate about which elements to select • Often require a lot less code than older DOM methods • Are already used by most front-end developers jQuery even adds some extra CSS-style selectors which offer additional functionality. Since jQuery was created, modern browsers have implemented the querySe 1 ector () and querySe 1ectorA11 () methods to let developers select elements using CSS syntax. However, these methods are not supported in older browsers.


***COMMON TASKS IN LESS CODE*** 

There are some tasks that front-end developers need to do regularly, such as loop through the elements that have been selected. jQuery has methods that offer web developers simpler ways to perform common tasks, such as: • loop through elements • Add I remove elements from the DOM tree • Handle events • Fade elements into I out of view • Handle Ajax requests jQuery simplifies each of these tasks, and allows you to write less code to achieve them. jQuery also offers chaining of methods (a technique which you will meet on p311). Once you have selected· some elements, this allows you to apply multiple methods to the same selection.


***CROSS-BROWSER COMPATIBILITY***

 jQuery automatically handles the inconsistent ways in which browsers select elements and handle events, so you do not need to write cross-browser fa llback code (such as that shown in the previous two chapters). To do this, jQuery uses feat ure detection to find the best way to achieve a task. It involves the use of many conditional statements: if the browser supports the ideal way to achieve a task, it us.es that approach; otherwise, it tests to see if it supports the next best option to achieve the same task.


***UPDATING ELEMENTS***

Here are four methods that update the content of all elements in a jQuery selection.##
. html()
. text()
.replaceWith()
. remove()


***INSERTING ELEMENTS***


.before()
.after()
.prepend()
.append()


# Pair Programming


How does pair programming work? While there are many different styles, pair programming commonly involves two roles: the Driver and the Navigator. The Driver is the programmer who is typing and the only one whose hands are on the keyboard. Handling the “mechanics” of coding, the Driver manages the text editor, switching files, version control, and—of course writing—code. The Navigator uses their words to guide the Driver but does not provide any direct input to the computer. The Navigator thinks about the big picture, what comes next, how an algorithm might be converted in to code, while scanning for typos or bugs. The Navigator might also utilize their computer as a second screen to look up solutions and documentation, but should not be writing any code.


1. Why pair program?

2. Greater efficiency

3. Engaged collaboration

4. Learning from fellow students

5. Social skills

6. Job interview readiness