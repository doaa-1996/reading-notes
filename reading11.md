
# EJS

EJS simply stands for Embedded Javascript. It is a simple templating language/engine that lets its user generate HTML with plain javascript.

Basic Syntax(Tags)

1. <% 'Scriptlet' tag, for control-flow, no output
2. <%= Outputs the value into the template (HTML escaped)
3. <%- Outputs the unescaped value into the template




## Get Started


***Install***


It's easy to install EJS with NPM.

**$ npm install ejs**


***Use***

Pass EJS a template string and some data.

let ejs = require('ejs');

let people = ['geddy', 'neil', 'alex'];

let html = ejs.render('<%= people.join(", "); %>', {people: people});


***CLI***

Feed it a template file and a data file, and specify an output file.


ejs ./template_file.ejs -f data_file.json -o ./output.html


***Browser support***

Download a browser build from the latest release, and use it in a script tag.


<script src="ejs.js"></script>

<script>

  let people = ['geddy', 'neil', 'alex'];

  let html = ejs.render('<%= people.join(", "); %>', {people: people}
  
  );

</script>

