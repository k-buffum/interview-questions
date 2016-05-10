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
  - Language & framework: Ruby on Rails
  - Database: Sql
  - Text Editor: Sublime

* Which version control systems are you familiar with?
  - Git

* Can you describe your workflow when you create a web page?
  - When creating a web page I begin by creating ERB's, wireframes, and user stories.
  - Once those are complete, I create the database, followed by basic functionality, ending with styling.

* If you have 5 different stylesheets, how would you best integrate them into the site?
  - I'm not sure why I would have 5 different stye sheets. It seems a bit excessive when you can put all of the information on one page dividing it into sections based on the page you are styling.
  - But, if I did encounter this problem I would just include the link tags on the layout.html page or the pages using those stylings.

* Can you describe the difference between progressive enhancement and graceful degradation?
  - Progressive enhancement: Giving a client the simplest site and functionality and adding fancy functionality for users with newer browsers
  - Graceful degradation: Moving from mobile, laptop, crappy phone, fancy tablet seamlessly, and the web page works well and looks well on each.

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
  - HTML (HyperText Markup Language) was the first standard to be created. It serves as the 'backbone of WWW', and is 'the most common tool used to design web pages'. (http://www.sitepoint.com/importance-web-standards/)
  - XHTML (eXtensible HyperText Markup Language) is an improved strict version of HTML. XHTML requires '!DOCTYPE', html, title, and body tags in the body of the html file. All tags must be closed and attributes must be lowercase and have quotes.

* What are `data-` attributes good for?
  - They are good for adding style to HTML

* Describe the difference between a `cookie`, `sessionStorage` and `localStorage`.
  - 'cookie' : small text files stored on your computer, helps the web page remember user information
  - 'sessionStorage' : data stored in sessionStorage gets cleared when the page session ends, allows you to access a session Storage object
  - 'localStorage' : stores user info on their local machine

* Why is it generally a good idea to position CSS `<link>`s between `<head></head>` and JS `<script>`s just before `</body>`? Do you know any exceptions?
  - The CSS <link> tags are in the <head></head> tags  because it will load first on the page, the JS <script> tags are before the </body> tag so that the page loads gracefully even if the JS isn't fully loaded.

## CSS Questions

* What is the difference between classes and IDs in CSS?
  - ID's are used to identify 1 item on the page you want styled differently
  - Classes are used to style a group of items on a page

* What's the difference between "resetting" and "normalizing" CSS? Which would you choose, and why?
  - Resetting: resets the HTML styling to a consistent baseline
  - Normalizing: similar to resetting, but only targets styles that need normailizing 

* Describe Floats and how they work.
  - Float is an css attribute that moves the object you are styling to the left or right side of the webpage.

* Describe z-index and how stacking context is formed.
  - Used for positioning elements on a page (stacking them), often inherits from the parent element. If the z-index is "-" (negative) the item is moved to the bottom of the stack so other elements can be stacked on top of it.

* Have you ever used a grid system, and if so, what do you prefer?
  - Yes, bootstrap columns (the only one I have used).

* Have you used or implemented media queries or mobile specific layouts/CSS?
  - Yes, @media(min-width:500px){}

* How do you optimize your webpages for print?
  - Create a print.css file
  - Remove header, footer, side bars, any unneccisary information that doesn't pertain to the main content of the article or page.

* What are the advantages/disadvantages of using CSS preprocessors?
  * Describe what you like and dislike about the CSS preprocessors you have used.
    - Advantages: Quick solution for styling, great options for people who don't know how to customize CSS to similar specifications
    - Disadvantages: Most websites that use these look similar, they are not unique in design.  As a developer you can come to rely on these tools and forget how to customize styling

* How would you implement a web design comp that uses non-standard fonts?
  - I would use Google Fonts by including a link in the header of my HTML document, and implementing it in my CSS file.

* Explain how a browser determines what elements match a CSS selector.
  - A browser can match elements and CSS selectors in many ways.  Some examples are using id's, classes, element names, before and after, links, etc.

* Explain your understanding of the box model and how you would tell the browser in CSS to render your layout in different box models.
  - A box model is used to add padding, border, and margin to an element.  It determines how much space an element takes up on a page. You can make box models different for each element by using classes or id's to associate the CSS styling applicable to that element.

* What does ```* { box-sizing: border-box; }``` do? What are its advantages?
  - It set's the box sizing of all elements to be the width and height assigned to that element, the padding doesn't alter the height or width of element.

* List as many values for the display property that you can remember.
  - inline-block
  - block
  - inline
  - web-kit-inline-block
  - web-kit-inline
  - web-kit-block
  - web-kit-box
  - flex
  - grid
  - inherit
  - none
  - initial
  - inline-flex

* What's the difference between inline and inline-block?
  - inline: displays items horizontally
  - inline-block: displays items horizontally, but if the elements have child elements those items are displayed vertically

* What's the difference between a relative, fixed, absolute and statically positioned element?
  - absolute: Allows you to place an element anywhere on the page, use top, bottom, left, right, to set the position. Positioning is relative to the parent element. The element will not effect any other elements on a page and vise versa.
  - relative: With no other positioning such as top, bottom, etc, this does nothing. BUT if you use "top: 10px" in addition to "position: relative", it will move the element down 10px. If this is used by itself it will use a z index and be placed ontop of static elements.
  - fixed: Positions the element to a certain spot on the page, the element doesn't move if the page is scrolling. ex) a sticky nav, nav stays positions at top of page if page is scrolled to bottom.
  - static: Positions the element to flow with the page, nothing special.. go with the flow

* The 'C' in CSS stands for Cascading.  How is priority determined in assigning styles (a few examples)?  How can you use this system to your advantage?
  - Priority is determined in CSS by using the bottom most styling that relates to an element on the page. For example..
    div {
      top:0;
      right: 0;
    }

    div {
      bottom:0;
      left: 0;
    }
  - The bottom div styling will be applied to all divs and no div will have the first div styling. This can be an advantage when using media queries.

* What existing CSS frameworks have you used locally, or in production? How would you change/improve them?
  - Bootstrap, Materialize
  - I find them very useful the way they are, I like that you can customize them and aren't stuck with a set style while using either. They are great tools!

* Have you played around with the new CSS Flexbox or Grid specs?
  - I have only played with CSS Flexbox when completing a Flexbox Froggy assignment.

* Have you ever worked with retina graphics? If so, when and what techniques did you use?
  - No

* Explain some of the pros and cons for CSS animations versus JavaScript animations.
  - 

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
- function Person(){} : defining a function named Person
- var person = Person() : sets person equal to the result of the function Person
- var person = new Person() : creating a new Person

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
- 

## Database Questions

* Design a database schema for Facebook, with at least 4 models, a complete set of attributes for each model, a 1:M association, and a M:M association.
  Associations:
  - User(one) to Post(many)
  - User(one) to Comment(many)
  - User(one) to Friends(many)
  - User(many) to UserGroup(one)
  - Group(many) to UserGroup(one)
  - Post(one) to Comment(many)
  - Post(one) to Like(many)
  - Comment(one) to Like(many)

  DB Schema/ models:
  - User: id, name, default photo, email, password
  - Post: id, content, user_id
  - Comment: id, body, user_id, post_id, parent_id
  - Friends: id, user_id, friend_id
  - Like: id, user_id, media_type, media_id, like_type
  - Group: id, name, description
  - GroupUsers: id, group_id, user_id


## Ruby/Rails
* What are ruby gems?
* What is the difference between a symbol and a string?
* What is the difference between a class method and an instance method?
* What is the difference between local variables, instance variables, and class variables?
* What is a range?

* In ruby, what does attr_accessor do?
- Allows the information to the right side of att_accessor to be accessed by users (read, write, edit)

* What is the purpose of environment files under the config folder in Rails? (development, test, production)
* What is the purpose of the application.rb file in Rails?
* How can you define a constant?
* What is the purpose of `yield`?

* How do you store API keys when creating an app?
- Place your API key in a ".env" file and use the key by calling the key name

* How do I send parameters through a url?
* Explain MVC

* What is a `before_action`? When would you use it?
- Something you put on a controller that gets executed before any functions or pages get activated, you would use it to see if a person has access to a page if they are(n't) logged in.

* What do controllers do in rails?
* What is RESTful routing?
* What is a polymorphic association?
* What are params?
* How do I make a migration to add a column in Rails?

* What is CSRF? How does Rails protect an app against this?
- Cross-Site Request Forgery
- Stores user information in a cookie, (sessions), restricts access to page based on what cookie is on the users machine. Uses a new token for each user login

* What's the difference between `User.find_by_id(1)` and `User.find(1)`?
- User.find_by_id(1) : finds a user in the User DB with the id of 1
- User.find(1) : finds the first user in the User DB

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
  - 1020

*Question: How would you make this work?*
```javascript
add(2, 5); // 7
add(2)(5); // 7
```
  - function add (a, b) {
      return a + b;
    }

*Question: What value is returned from the following statement?*
```javascript
"i'm a lasagna hog".split("").reverse().join("");
```
  - "goh angasal a m'i"

*Question: What is the outcome of the two alerts below?*
```javascript
var foo = "Hello";
(function() {
  var bar = " World";
  alert(foo + bar);
})();
alert(foo + bar);
```
  - "Hello World"

*Question: What is the value of `foo.length`?*
```javascript
var foo = [];
foo.push(1);
foo.push(2);
```
  - 2

*Question: What is the value of `foo.x`?*
```javascript
var foo = {n: 1};
var bar = foo;
foo.x = foo = {n: 2};
```
- undefined

*Question: What does the following code print?*
```javascript
console.log('one');
setTimeout(function() {
  console.log('two');
}, 0);
console.log('three');
```
- "one", "three", "two"

## Fun Questions:

* What's a cool project that you've recently worked on?
* What are some things you like about the developer tools you use?
* Do you have any pet projects? What kind?
* How do you like your coffee?
