<!-- 
---
title: Persisting Form Input with jQuery and Browser Storage
type: lesson
duration: "1:25"
creator:
    name: Ben Hulan
    city: SF
competencies: Front-end intro
adapted by: 
    name: Zeb Girouard
    city: DEN
---
 -->

<!-- Hook: So...you're filling out a form for something: taxes, registration, or a sign-up for a website.  You realize you made a mistake, so you hit the back button...but that takes you all the way to the beginning.  And worse yet, all your information is now gone.  You have to start all over again. Raise your hand if this has happened to you.  

Today we will talk about one way to resolve this headache, with localStorage.

Another headache you may be familiar with is from the LOTR lab.  Remember having to remember all those complex commands for selecting IDs, classes, and attributes?  

Well, with jQuery we'll make that process a lot easier.
-->

# Persisting Form Input with jQuery and Browser Storage

<!-- 9:00 -->

### Objectives
*After this lesson, students will be able to:*

- **Import** jQuery to a webpage
- **Construct** a jQuery selector
- **Create** HTML forms and store user input in the browser
- **Read** and **write** data with localStorage and sessionStorage
- **Understand** the pros and cons of using built-in browser storage

### Preparation
*Before this lesson, students should already be able to:*

- **Write** basic HTML/CSS
- **Read** and **write** basic vanilla Javascript

<!-- CFU Fist-to-five on these concepts -->

### Why do we need localStorage?
In this Unit we will be building Browser games with HTML, CSS and client-side JavaScript. Although we are not yet ready to connect a database on the backend or store data on a server, the browser offers the ability to persist data locally using `sessionStorage`, `localStorage` and some other options we may explore later in the course.

Creating a game, you may wish to allow your users to store their names and high scores, or keep track of some other simple data.

[Here](https://developer.mozilla.org/en-US/docs/Web/API/Storage) is a look at some documentation for the Web Storage API.

## Intro to jQuery (15 min)

<!-- 9:05 -->

### What is jQuery?

**jQuery** is a Javascript library with a lot of useful pre-defined functions and expressions.  Basically you can think of it as a very large chunk of Javascript code that you add to your webpage *before* you add your own Javascript, so you can use all these functions and expressions in your own code.

### Importing jQuery in `index.html`

In order to start with **jQuery**, you need to copy this somewhere on your HTML page, *above* the script import tag of your own Javascript, like this:

```html

<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.0.0-rc1/jquery.min.js"></script>
<script src="myjavascript.js"></script>

```

### What is "$"

One of the most important pieces of jQuery is the `$` sign.  This is an alias for `jQuery`, and it means "access the jQuery library to do something".  Here are a few examples:

```javascript

$("body").hide(); // Hides the body of your page
$(".link").css("color", "red"); // Turns all links red
$(document).ready(function(){

   // Yay our page loaded!!
   // jQuery methods go here...

});
```

### jQuery Selectors

Typical jQuery syntax has three parts:
 - A $ sign to define/access jQuery
 - A (selector) to "query (or find)" HTML elements
 - A jQuery action() to be performed on the element(s)
 
jQuery selectors fall into the same categories as the CSS selectors you have already seen.  Most importantly:
 - Tag Name (e.g. "p", "h1", "body")
 - Class (e.g. ".default-button", ".col-md-6")
 - ID (e.g. "#catPicture", "#student26")
 
So what would I write if I wanted to change student26's background color to blue?

### Independent Practice (10 min)

<!-- 9:30 -->

Take a minute to think out the following steps.  In pairs, complete the following steps:

 - Create a boilerplate index.html page (remember the <h + `tab` trick in Sublime?)
 - Import jQuery (Hint: use the line above)
 - Create a heading tag (h1, h2, or h3)
 - Give it a class
 - Create an inline-style tag below your jQuery import
 - Use jQuery to select this heading, and change its color

Bonus:

 - If you have time, use jQuery to select another element, and change its positioning or size

## Warm-up (15 min)

<!-- 9:40 -->

Before we begin, let's look at the files in `browser-storage-examples`. 
`sessionStorage.html` is the most basic. We will go through this line-by-line in class.
`localStorage1.html` does the same thing, but it adds the clear button.
`localStorage2.html` takes things a bit farther. Take a look at the code and _without opening it in the browser_ see if you can explain what's happening.

<!-- CFU: Think-pair-share to explain what's happening on 2nd file -->

Let's brainstorm some other tasks we can accomplish with localStorage or sessionStorage

## Instructions:

<!-- 9:55 -->

- Divide into groups of 3-4
- Figure out something to keep track of on a simple single-page web app
- Create a Form with the <form></form> tag
- Save the info to localStorage
- Feel free to "borrow" liberally from the example code in the repo


_Remember: `localStorage` and `sessionStorage` only store strings, so you may need to `parseInt()` if you need to do anything with the user data after it has been entered._

## Resources:

[jQuery Intro on W3Schools](http://www.w3schools.com/jquery)
