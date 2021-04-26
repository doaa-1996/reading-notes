# APIs

***What is REST?***

REST is acronym for Representational State Transfer. It is architectural style for distributed hypermedia systems and was first presented by Roy Fielding in 2000 in his famous dissertation.

***Principles of REST***

Client–server
Stateless
Cacheable
Uniform interface
Layered system
Code on demand


***Resource Methods***

GET/PUT/POST/DELETE


***REST and HTTP are not same***

Representational state transfer (REST) is a software architectural style that defines a set of constraints to be used for creating Web services. Web services that conform to the REST architectural style, called RESTful Web services, provide interoperability between computer systems on the Internet. RESTful Web services allow the requesting systems to access and manipulate textual representations of Web resources by using a uniform and predefined set of stateless operations. Other kinds of Web services, such as SOAP Web services, expose their own arbitrary sets of operations.

The Hypertext Transfer Protocol (HTTP) is an application protocol for distributed, collaborative, hypermedia information systems. HTTP is the foundation of data communication for the World Wide Web, where hypertext documents include hyperlinks to other resources that the user can easily access, for example by a mouse click or by tapping the screen in a web browser.


***Building a simple REST API with NodeJS and Express***

Initialize a new app:

$ npm init

The first way is creating the files by hand. A basic Node app contains a .js file and a package.json file. The package.json file contains a couple of properties. First one is name which holds the name of the app, second is version which shows the version of your app, a description of your app, main that points to the entry point of your application. There’s also scripts, that can be run when you need to perform some repetitive tasks, author name, licence, dependencies and devDependencies.


Install Express:

'npm install express'

Creating the app:

hen create the app.js file or whatever you prefer naming it (default is index.js) and add in the following code.

var express = require("express");
var app = express();

app.listen(3000, () => {
 console.log("Server running on port 3000");
});

app.get("/url", (req, res, next) => {
 res.json(["Tony","Lisa","Michael","Ginger","Food"]);
});
Running your app:

To run your app, use the command below.

npm start


***SuperAgent***

SuperAgent is light-weight progressive ajax API crafted for flexibility, readability, and a low learning curve after being frustrated with many of the existing request APIs. It also works with Node.js!



