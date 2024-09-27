---
layout: essay
type: essay
title: "The Importance of Coding Standards"
# All dates must be YYYY-MM-DD format!
date: 2024-09-26
published: true
labels:
  - ESLint
  - Javascript
  - Typescript
---

<img class="img-fluid" src="../img/coding/coding-header.png">

# What even is ESLint?

ESLint is a code analysis tool that’s used to identify problems in both Javascript and Typescript. It catches in on errors that might seem trivial to the typical programmer, but it’s useful in maintaining a well-organized environment. The “lint” in ESLint refers to linting, and it’s the programmer's word for picking up on syntactical and styling issues. In class, we installed ESLint by first downloading VSCode, and then downloading Node, which is a Javascript runtime. Then, we installed ESLint by doing an npm install in the project directory.

It’s a tiny thing to do, and it’s just one Node package, but it can be powerful when reviewing code. It’s a tool that should be utilized everywhere in the coding world because I feel like styling is something that should be standard across the board. Sometimes when I review my friend’s code or a classmate’s code, I see a bunch of varying styles. Maybe sometimes the opening curly bracket is placed on the same line, or it’s placed on a new line. Maybe their spacing or tab widths vary wildly in the same file. All these can be fixed by having ESLint be a standard everywhere.

Here’s an example of the kinds of things the linter catches:

```
console.log("Hello") // Strings must use singlequote.
let a = 3; // a is never reassigned. Use ‘const’ instead.
let b; // b is defined but never used.
```

# My stance on ESLint

When I first installed ESLint and did the assignment where I had to fix all the syntax issues, it was a little tedious. It picked up on the smallest of things. If I forgot a new line at the end of my file, it threw an error. If I made my tabs four spaces instead of two, there were errors on every line. To add on, when I would do the in-class WODs every Thursday, I would need to make sure that my code was perfect before running it. ESLint caught every single tiny error I made, and it was a little daunting seeing two-digit numbers of errors after I finished my code. However, I got to sort of appreciate ESLint. It reminded me of the things I forgot to put. Maybe I used let instead of const for a variable that doesn’t change, or I forgot to define the return statement for a non-void function. It helped keep my code clean and in check.

ESLint sort of reminded me of my ICS212 teacher, Ravi. He had an entire page on his course website that listed what he expected stylistically when the TAs graded our coding assignments. Some of the things on the list included things like no global variables, listing all the local variables at the start of the function/method, having a header comment for every function/method, and using four spaces for every indent. The rules he laid out for the styling were akin to ESLint, and it made my C code quite clean.

# In conclusion...

All in all, I think ESLint is a very useful tool that should be in the back pocket of any software engineer. It makes code bases clean and allows for a well-designed standard to follow when it comes to style choices.