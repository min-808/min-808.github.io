---
layout: essay
type: essay
title: "UI Frameworks and Their Convenience"
# All dates must be YYYY-MM-DD format!
date: 2024-10-10
published: true
labels:
  - HTML
  - CSS
  - Bootstrap 5
---

<img class="img-fluid" src="../img/ui-frameworks/bootstrap-header.png">

# What is a UI framework?

A UI framework is an important part of front-end development and is what most modern websites today rely on. Essentially, it’s a collection of pre-built components, like headers and containers, that help developers make website user interfaces more effective. They help with providing standardized ways to build and manage the layout and design of an application. Furthermore, instead of starting from scratch every time you want to make a website, these frameworks provide an easier way to style a website's components and focus more on functionality and ease of use. An example of a UI framework is Bootstrap 5, and it’s something we’ve been using in class for some time now. Other UI frameworks include React, Angular, and Vue.

# Why use UI frameworks?

When I was starting web development, I was in my high school coding class learning about the basics of HTML and CSS. There were so many elements and so many styling options to each element, that I felt like I got a bit overwhelmed. In addition, there were things like flex boxes, absolute positioning, and concepts like z-indexing and window compatibility that really confused me. I got pretty frustrated when my website would work well on my computer, but if I were to load it up on a school Chromebook, all the elements would be in the wrong places.

For the next few years, whenever I wanted to make a website of my own, I would rely on pure HTML and CSS to build them. It was the only way I knew how to build websites, and it was reliable for the most part.

<img class="img-fluid" src="../img/ui-frameworks/seele-web.png">

This was the home page of the [Seele Bot](https://min-808.github.io/projects/seele.html) mentioned in my projects page. I styled it with basic HTML and CSS elements, and I remember being somewhat irked when the divs wouldn’t center or when the header didn’t look right.

Now, fast forward to the present where we’re learning about Bootstrap 5, and I feel like life has become much easier. I was pretty shocked that we could just include two files, and create responsive and interactive components on the spot. To create a navigation bar at the top of the page, you can simply do:

```
<nav class="navbar navbar-expand-lg navbar-light bg-light">
```

To explain what the syntax means: 

- navbar-expand-lg means that the nav bar should collapse once the viewport shrinks to the size indicated by lg (992px)
- navbar-light means that the nav bar should have the light theme with dark text
- bg-light sets the light background of the nav bar

And to add elements within the navbar, you can enclose nav items items inside of a container:

```
<div class="container-fluid">
  <ul class="navbar-nav">
    <li class="nav-item">
    </li>
    <li class="nav-item">
    </li>
    <li class="nav-item">
    </li>
  </ul>
</div>
```

- container-fluid means that the div should take up the whole width of the viewport, allowing for proper spacing on the sides

There are also lots of minor things that can be done to improve the look of a page. Padding and margins are simplified to m and p flags where the sizes can be changed in-line.

# In conclusion...

I think UI frameworks are a necessary part of learning web development and are crucial in making websites clean and functional. Furthermore, by learning UI frameworks, it’s easy to start a website from scratch, and even migrate older websites to a more robust and well-maintained framework. In future web development jobs, it may even be required to learn web frameworks to keep up with maintaining websites and working in teams.