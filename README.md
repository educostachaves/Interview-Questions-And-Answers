# Interview questions and your answers

This is only a simple review of some questions that may you will receive from a interviewer. It isn't a clue, but my intention is study each question, not only to answer, but be a better developer.

General Questions:

- Are you on Twitter?
Yes. you need use twitter, not to post usual things, like drink a coffee, or wash your hands, but follow developers of technologies that you like.
- If so, who do you follow on Twitter?
Good international names: Brendan Eich [@BrendanEich](https://twitter.com/BrendanEich), Chris Heilmann
[@codepo](https://twitter.com/codepo8), James Halliday [@substack](https://twitter.com/substack), Sebastian McKenzie [@sebmck](https://twitter.com/sebmck), Laurie Voss [@seldo](https://twitter.com/seldo)
Good Brazilian Names: 
- Are you on GitHub?
Yes! You must have a GitHub Account.
- If so, what are some examples of repos you follow
- What blogs do you follow?
- What version control systems have you used (Git, SVN etc.)?
- What is your preferred development environment? (OS, Editor, Browsers, Tools etc.)
- Can you describe your workflow when you create a web page?
- Can you describe the difference between progressive enhancement and graceful degradation?
- Bonus points for describing feature detection
- Explain what "Semantic HTML" means.
- What browser do you primarily develop in and what developer tools do you use?
- How would you optimize a websites assets/resources?
- Looking for a number of solutions which can include:
- File concatenation
- File minification
- CDN Hosted
- Caching
etc.

Why is it better to serve site assets from multiple domains?
How many resources will a browser download from a given domain at a time?
Name 3 ways to decrease page load. (perceived or actual load time)
If you jumped on a project and they used tabs and you used spaces, what would you do?
Suggest the project utilize something like EditorConfig (http://editorconfig.org)
Conform to the conventions (stay consistant)
issue :retab! command
Write a simple slideshow page
Bonus points if it does not use JS.
What tools do you use to test your code's performance?
JSPerf (http://jsperf.com/)
Dromaeo (http://dromaeo.com/)
etc.
If you could master one technology this year, what would it be?
Explain the importance of standards and standards bodies.
What is FOUC? How do you avoid FOUC?
HTML-Specific Questions:

What's a doctype do, and how many can you name?
What's the difference between standards mode and quirks mode?
What are the limitations when serving XHTML pages?
Are there any problems with serving pages as application/xhtml+xml?
How do you serve a page with content in multiple languages?
What kind of things must you be wary of when design or developing for multilingual sites?
Can you use XHTML syntax in HTML5?
How do you use XML in HTML5?
What are data- attributes good for?
What are the content models in HTML4 and are they different in HTML5?
Consider HTML5 as an open web platform. What are the building blocks of HTML5?
Describe the difference between cookies, sessionStorage and localStorage.
JS-Specific Questions

Which JavaScript libraries have you used?
Have you ever looked at the source code of the libraries/frameworks you use?
How is JavaScript different from Java?
What's a hashtable?
What are undefined and undeclared variables?
What is a closure, and how/why would you use one?
Your favorite pattern used to create them? argyle (Only applicable to IIFEs)
What's a typical use case for anonymous functions?
Explain the "JavaScript module pattern" and when you'd use it.
Bonus points for mentioning clean namespacing.
What if your modules are namespace-less?
How do you organize your code? (module pattern, classical inheritance?)
What's the difference between host objects and native objects?
Difference between:
function Person(){} var person = Person() var person = new Person()
What's the difference between .call and .apply?
explain Function.prototype.bind?
When do you optimize your code?
Can you explain how inheritance works in JavaScript?
When would you use document.write()?
Most generated ads still utilize document.write() although its use is frowned upon
What's the difference between feature detection, feature inference, and using the UA string
Explain AJAX in as much detail as possible
Explain how JSONP works (and how it's not really AJAX)
Have you ever used JavaScript templating?
If so, what libraries have you used? (Mustache.js, Handlebars etc.)
Explain "hoisting".
Describe event bubbling.
What's the difference between an "attribute" and a "property"?
Why is extending built in JavaScript objects not a good idea?
Why is extending built ins a good idea?
Difference between document load event and document ready event?
What is the difference between == and ===?
Explain how you would get a query string parameter from the browser window's URL.
Explain the same-origin policy with regards to JavaScript.
Explain event delegation.
Describe inheritance patterns in JavaScript.
Make this work:
[1,2,3,4,5].duplicator(); // [1,2,3,4,5,1,2,3,4,5]
Describe a strategy for memoization (avoiding calculation repetition) in JavaScript.
Why is it called a Ternary statement, what does the word "Ternary" indicate?
What is the arity of a function?
What is "use strict";? what are the advantages and disadvantages to using it?
JS-Code Examples:

~~3.14
Question: What value is returned from the above statement? Answer: 3

"i'm a lasagna hog".split("").reverse().join("");
Question: What value is returned from the above statement? Answer: "goh angasal a m'i"

( window.foo || ( window.foo = "bar" ) );
Question: What is the value of window.foo? Answer: "bar" only if window.foo was falsey otherwise it will retain its value.

var foo = "Hello"; (function() { var bar = " World"; alert(foo + bar); })(); alert(foo + bar);
Question: What is the outcome of the two alerts above? Answer: "Hello World" & ReferenceError: bar is not defined

var foo = [];
foo.push(1);
foo.push(2);
Question: What is the value of foo.length? **Answer: 2

var foo = {};
foo.bar = 'hello';
Question: What is the value of foo.length? **Answer: undefined

foo = foo||bar
Question: What is the mean for? **Answer: if(!foo) foo = bar

foo>>1
Question: What is the mean for? **Answer: Math.floor(foo/2)

foo|0
foo+.5|0
Question: What is the mean for? **Answer: parseInt(foo) & Math.round(foo)

function foo(bar1, bar2, bar3){}
Question: How to get the numbers of parameters? **Answer: foo.length //this example is 3

jQuery-Specific Questions:

Explain "chaining".
Explain "deferreds".
What are some jQuery specific optimizations you can implement?
What does .end() do?
How, and why, would you namespace a bound event handler?
Name 4 different values you can pass to the jQuery method.
Selector (string), HTML (string), Callback (function), HTMLElement, object, array, element array, jQuery Object etc.
What is the effects (or fx) queue?
What is the difference between .get(), [], and .eq()?
What is the difference between .bind(), .live(), and .delegate()?
What is the difference between $ and $.fn? Or just what is $.fn.
Optimize this selector:
$(".foo div#bar:eq(0)")
Difference between 'delegate()' and 'live()'?
CSS-Specific Questions:

Describe what a "reset" CSS file does and how it's useful.
Describe Floats and how they work.
What are the various clearing techniques and which is appropriate for what context?
Explain CSS sprites, and how you would implement them on a page or site.
What are your favourite image replacement techniques and which do you use when?
CSS property hacks, conditionally included .css files, or... something else?
How do you serve your pages for feature-constrained browsers?
What techniques/processes do you use?
What are the different ways to visually hide content (and make it available only for screen readers)?
Have you ever used a grid system, and if so, what do you prefer?
Have you used or implemented media queries or mobile specific layouts/CSS?
Any familiarity with styling SVG?
How do you optimize your webpages for print?
What are some of the "gotchas" for writing efficient CSS?
Do you use CSS preprocessors? (SASS, Compass, Stylus, LESS)
If so, describe what you like and dislike about the CSS preprocessors you have used.
How would you implement a web design comp that uses non-standard fonts?
Webfonts (font services like: Google Webfonts, Typekit etc.)
Explain how a browser determines what elements match a CSS selector?
Optional fun Questions:

What's the coolest thing you've ever coded, what are you most proud of?
Do you know the HTML5 gang sign?
Are you now, or have you ever been, on a boat.
What are your favorite parts about the developer tools you use?
Do you have any pet projects? What kind?
Explain the significance of "cornify".
On a piece of paper, write down the letters A B C D E vertically. Now put these in descending order without writing one line of code.
Wait and see if they turn the paper upside down
Pirate or Ninja?
Bonus if it's a combo and a good reason was given (+2 for zombie monkey pirate ninjas)
If not Web Development, what would you be doing?
Where in the world is Carmen Sandiego?
Hint: their answer is always wrong
What's your favorite feature of Internet Explorer?
Complete this sentence: Brendan Eich and Doug Crockford are the __________ of javascript.
jQuery: a great library or the greatest library? Discuss.
http://www.w3schools.com/ or http://w3fools.com/
