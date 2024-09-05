---
layout: project
type: project
image: img/seele/seele-square.png
title: "Seele Discord Bot"
date: 2023
published: true
labels:
  - Javascript/Discord.JS
  - MongoDB
  - Github
  - Mongoose
summary: "A dynamic Discord bot game based on the game Honkai: Star Rail."
---

<img class="img-fluid" src="../img/vacay/vacay-home-page.png">

Seele is a Discord bot I spent Winter 2023 working on. This project helped me learn about Javascript, as well as how to structure a database schema.

Seele is implemented using [Discord.JS](https://discord.js.org/), a Node.js module that interacts with the Discord API very easily. Within three weeks, I created a fully-fledged bot that has an economy, various games, and a daily log-in system.

In this project I gained experience with [MongoDB](http://mongodb.com) for database storage, Javascript for creating the interactions, and Mongoose for creating a connection between MongoDB and the Node.js runtime environment.

Here is some example code to illustrate a simple example of writing to the database:

{% gist 82892cec7a5047c084ad2a5acc443812 %}

In this code snippet, the function **setUptime()** is an asynchronous function that is continuously called to set the uptime of the bot.
The function stores the current time in **currentTime** and connects to the database and finds the collection named **uptime**.
Once found, the **.updateOne** function is called in order to **set** the element called **time** to **currentTime**.
There are more complex functions to MongoDB, another example is shown below

{% gist a70b9d8faf2b9ff78ba34a17b8cc3ffc %}

Here, a series of actions take place utilizing the **.updateMany** function. First, the expression checks if one element is less than another.
This is done with the **$expr** and **lt** operators. If so, then the selected element is increased by 1.

Both **setUptime()** and **replenishPower()** are events that are called periodically using [Cron](https://www.npmjs.com/package/cron), a popular node package.



Source: <a href="https://github.com/theVacay/vacay">theVacay/vacay</a>
