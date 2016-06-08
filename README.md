<!-- 
---
title: Persisting Form Input with jQuery and Browser Storage
type: lesson
duration: "1:25"
creator:
    name: Ben Hulan
    city: SF
competencies: Front-end intro
adapted by: Zeb Girouard
---
 -->

<!-- Hook: So...you're filling out a form for something: taxes, registration, or a sign-up for a website.  You realize you made a mistake, so you hit the back button...but that takes you all the way to the beginning.  And worse yet, all your information is now gone.  You have to start all over again. Raise your hand if this has happened to you.  

Today we will talk about one way to resolve this headache, with localStorage.
-->

# Persisting Form Input with jQuery and Browser Storage

### Objectives
*After this lesson, students will be able to:*

- Create HTML forms and store user input in the browser
- Read and write data with localStorage and sessionStorage
- Understand the pros and cons of using built-in browser storage

### Preparation
*Before this lesson, students should already be able to:*

- Write basic HTML/CSS
- Read and write basic vanilla Javascript

### Why are we doing this?
In this Unit we will be building Browser games with HTML, CSS and client-side JavaScript. Although we are not yet ready to connect a database on the backend or store data on a server, the browser offers the ability to persist data locally using `sessionStorage`, `localStorage` and some other options we may explore later in the course.

Creating a game, you may wish to allow your users to store their names and high scores, or keep track of some other simple data.

[Here](https://developer.mozilla.org/en-US/docs/Web/API/Storage) is a look at some documentation for the Web Storage API.

## Warm-up (15 min)
Before we begin, let's look at the files in `browser-storage-examples`
`sessionStorage.html` is the most basic. We will go through this line-by-line in class.
`localStorage1.html` does the same thing, but it adds the clear button.
`localStorage2.html` takes things a bit farther. Take a look at the code and _without opening it in the browser_ see if you can explain what's happening.

<!-- CFU: Think-pair-share to explain what's happening on 2nd file -->

Let's brainstorm some other tasks we can accomplish with localStorage or sessionStorage

## Instructions:

- Divide into groups of 3-4
- Figure out something to keep track of on a simple single-page web app
- Build it!


_Remember: `localStorage` and `sessionStorage` only store strings, so you may need to `parseInt()` if you need to do anything with the user data after it has been entered._
