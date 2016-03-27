#Interview Prep

(Partially from https://github.com/h5bp/Front-end-Developer-Interview-Questions)

Go through all of the following questions and think about how you would respond to each. You should be able to answer many of the questions from memory, but you may have to research a few of them.

**Copy this md file to your homework folder and add a short answer under each item.** You should try to be as concise as possible, and list any handy resources you used to answer the question. This will be useful for studying for interviews after class.

## General Questions

* What did you learn yesterday/this week?
  - Yesterday I learned how to create custom filters and directives for Angular
  - This week I learned how to make a MEAN stack application

* What excites or interests you about coding?
  - Looking at and using my finished products are what excites me about coding.
  - One of the reasons I am interested in coding is because I can create products that people can use to learn and potentially help advance health technologies

* What is a recent technical challenge you experienced and how did you solve it?
  - A recent technical challenge I faced was creating a MEAN stack application for a day long hackathon.
  - I was working in a group with 3 other people and we tackeled this problem by first creating the models and controllers, then we data scraped a website, set up login/ signup functionality, created the front end, and finally set up a page to display the scraped data.

* What UI, Security, Performance, SEO, Maintainability or Technology considerations do you make while building a web application or site?
  - If I am creating a web app or site that requires a user to login I make sure to include restricted access to certain pages/ information and bcrypt to protect user passwords.
  - I also try to make my apps as easy to use as possible, if I feel a user will question someting I try to alter my front end code so that the functionality in question is self explanitory.
  - I try to keep my app as maintainable as possible by naming functions, id's, etc. by their use and what they do.
  - When taking SEO into consideration I try to name my routes as relevent to what the app is used for as possible.

* Talk about your preferred development environment.
  - I prefer to work in a quite, relaxed environment, that promotes learning and doesn't make you feel awkward for asking questions.

* Which version control systems are you familiar with?
  - Git

* Can you describe your workflow when you create a web page?
  - When creating a web page I begin by creating ERB's, wireframes, and user stories.
  - Once those are complete, I create the database, followed by basic functionality, ending with styling.

* If you have 5 different stylesheets, how would you best integrate them into the site?
  - I'm not sure why I would have 5 different stye sheets. It seems a bit excessive when you can put all of the information on one page dividing it into sections based on the page you are styling.
  - But, if I did encounter this problem I would just include the link tags on the layout.html page or the pages using those stylings.

* Can you describe the difference between progressive enhancement and graceful degradation?
  - Progressive enhancement: a web design strategy that emphasizes accessibility, sematic HTML markup, and external stylesheet and scrypting technologies
  - Graceful degradation: the ability of a computer, machine, electronic system, or network to maintain limited functionality even when a large portion of it has been destroyed or rendered inoperative. (NOT when Github went down) 

* Describe how you would create a simple slideshow page, without any frameworks (HTML/CSS/JS only).
  - In my HTML document I would create a div to display the slide show.
  - Using JS I would create an array with the different slide information, then create a function using a for loop to iterate over the array, and finally using setInterval() to set the length of time between slides.
  - CSS would be used to size and add style to the slide show so that it isn't displayed ugly and awkward against the left side of the page.

* If you could master one technology this year, what would it be?
  - Ruby on Rails

* Explain the importance of standards and standards bodies.
  - Standards were initiated due to the lack of structure when the web was first built.  Standards enable a site to be viewed on different browsers no matter how old they are. Without these, big companies could take over the web market and enable their content to only be viewed on their products, potentially monopolizing the web. (http://www.sitepoint.com/importance-web-standards/)

## HTML Questions

* What does a `doctype` do?
  - It tells the browser what version of the markup language the page is written in

* What's the difference between HTML and XHTML?
  -

* What are `data-` attributes good for?
  -

* Describe the difference between a `cookie`, `sessionStorage` and `localStorage`.
  -

* Why is it generally a good idea to position CSS `<link>`s between `<head></head>` and JS `<script>`s just before `</body>`? Do you know any exceptions?
  -

## CSS Questions

* What is the difference between classes and IDs in CSS?
* What's the difference between "resetting" and "normalizing" CSS? Which would you choose, and why?
* Describe Floats and how they work.
* Describe z-index and how stacking context is formed.
* Have you ever used a grid system, and if so, what do you prefer?
* Have you used or implemented media queries or mobile specific layouts/CSS?
* How do you optimize your webpages for print?
* What are the advantages/disadvantages of using CSS preprocessors?
  * Describe what you like and dislike about the CSS preprocessors you have used.
* How would you implement a web design comp that uses non-standard fonts?
* Explain how a browser determines what elements match a CSS selector.
* Explain your understanding of the box model and how you would tell the browser in CSS to render your layout in different box models.
* What does ```* { box-sizing: border-box; }``` do? What are its advantages?
* List as many values for the display property that you can remember.
* What's the difference between inline and inline-block?
* What's the difference between a relative, fixed, absolute and statically positioned element?
* The 'C' in CSS stands for Cascading.  How is priority determined in assigning styles (a few examples)?  How can you use this system to your advantage?
* What existing CSS frameworks have you used locally, or in production? How would you change/improve them?
* Have you played around with the new CSS Flexbox or Grid specs?
* Have you ever worked with retina graphics? If so, when and what techniques did you use?
* Explain some of the pros and cons for CSS animations versus JavaScript animations.

## JS Questions

* Explain event delegation
* Explain how `this` works in JavaScript
* Explain how prototypal inheritance works
* Why is it called a Ternary expression, what does the word "Ternary" indicate?
* What's the difference between a variable that is: `null`, `undefined` or `undeclared`?
  * How would you go about checking for any of these states?
* What is a closure, and how/why would you use one?
* What's a typical use case for anonymous functions?
* Difference between: `function Person(){}`, `var person = Person()`, and `var person = new Person()`?
* What's the difference between `.call` and `.apply`?
* Explain `Function.prototype.bind`.
* What's the difference between feature detection, feature inference, and using the User Agent string?
* Explain AJAX in as much detail as possible.
* Have you ever used JavaScript templating?
  * If so, what libraries have you used?
* Explain "hoisting".
* Describe event bubbling.
* What's the difference between an "attribute" and a "property"?
* Why is extending built-in JavaScript objects not a good idea?
* What is the difference between `==` and `===`?
* Explain the same-origin policy with regards to JavaScript.
* What is the extent of your experience with Promises and/or their polyfills?
* What are the pros and cons of using Promises instead of callbacks?
* What tools and techniques do you use debugging Javascript code?
* What language constructions do you use for iterating over object properties and array items?

## Database Questions

* Design a database schema for Facebook, with at least 4 models, a complete set of attributes for each model, a 1:M association, and a M:M association.

## Ruby/Rails
* What are ruby gems?
* What is the difference between a symbol and a string?
* What is the difference between a class method and an instance method?
* What is the difference between local variables, instance variables, and class variables?
* What is a range?
* In ruby, what does attr_accessor do?  
* What is the purpose of environment files under the config folder in Rails? (development, test, production)
* What is the purpose of the application.rb file in Rails?
* How can you define a constant?
* What is the purpose of `yield`?
* How do you store API keys when creating an app?
* How do I send parameters through a url?
* Explain MVC
* What is a `before_action`? When would you use it?
* What do controllers do in rails?
* What is RESTful routing?
* What is a polymorphic association?
* What are params?
* How do I make a migration to add a column in Rails?
* What is CSRF? How does Rails protect an app against this?
* What's the difference between `User.find_by_id(1)` and `User.find(1)`?
* What's are classes in Ruby? What are modules? And what's the difference?

## Testing Questions

* What are some advantages/disadvantages to testing your code?
* What tools would you use to test your code's functionality?
* What is the difference between a unit test and a functional/integration test?
* What is the purpose of a code style linting tool?
* What is End-to-end (E2E) testing? How can it be implemented in frameworks like Angular and Rails?

## Coding Questions:

*Question: What is the value of `foo`?*
```javascript
var foo = 10 + '20';
```

*Question: How would you make this work?*
```javascript
add(2, 5); // 7
add(2)(5); // 7
```

*Question: What value is returned from the following statement?*
```javascript
"i'm a lasagna hog".split("").reverse().join("");
```

*Question: What is the outcome of the two alerts below?*
```javascript
var foo = "Hello";
(function() {
  var bar = " World";
  alert(foo + bar);
})();
alert(foo + bar);
```

*Question: What is the value of `foo.length`?*
```javascript
var foo = [];
foo.push(1);
foo.push(2);
```

*Question: What is the value of `foo.x`?*
```javascript
var foo = {n: 1};
var bar = foo;
foo.x = foo = {n: 2};
```

*Question: What does the following code print?*
```javascript
console.log('one');
setTimeout(function() {
  console.log('two');
}, 0);
console.log('three');
```

## Fun Questions:

* What's a cool project that you've recently worked on?
* What are some things you like about the developer tools you use?
* Do you have any pet projects? What kind?
* How do you like your coffee?
