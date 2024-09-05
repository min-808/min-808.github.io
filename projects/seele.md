---
layout: project
type: project
image: img/seele/seele-square.png
title: "Seele Discord Bot"
date: 2023
published: true
labels:
  - Javascript
  - Discord.JS
  - MongoDB
  - Github
  - Mongoose
summary: "A dynamic Discord bot game based on the game Honkai: Star Rail."
---

<img class="img-fluid" src="../img/seele/seele-header4.png">

Seele is a Discord bot I spent the Winter of 2023 working on. The original purpose for this project was to pull profile data from a video game that I routinely played using their API. However, since the commands were very barebones and simple, I wanted to expand the project to involve more interactivity with the user. This led to me creating a whole game within the Discord bot that simulated the video game that I took inspiration from. I was able to create a fully-fledged bot that has an economy system, various mini-games, and daily login rewards to keep the players interested. This project helped me learn a lot about Javascript, as well as how to structure a database schema. In addition, I had to learn various parts of Discord's API and how bot messages are built, since they're different from user messages.

This project was a sole project intended for me to learn more about back-end development. I am responsible for all of the work, but I often looked to the Internet for guidance when I ran into issues. Some sources I utilized were the documentation and coding forums. Additionally, I watched multiple YouTube videos to kickstart the project since I had zero experience with Discord's bot system.

The main thing I learned from this project was Javascript. However, since the bot needed to interact with Discord's API, I had to pick up [Discord.JS](https://discord.js.org/) as well, a module that offers many helpful tools for bot creation. For the database, I used [MongoDB](http://mongodb.com) and learned about non-relational databases. The language used to interact with MongoDB is very different from languages like SQL. Since SQL databases store data in tables containing rows and columns, NoSQL databases like MongoDB store data in documents. These documents can have flexible schemas unlike SQL tables which must have a strict, predefined schema.

Here is some example code to illustrate an example of writing to the database:

```javascript
async function setUptime() {
    var currentTime = Date.now()

    var client = new MongoClient(uri)

    var database = client.db("economy")
    var ids = database.collection("uptime")

    await ids.updateOne({}, {
        $set: {
            time: currentTime
        }
    })
}
```

In this code snippet, the function **setUptime()** is an asynchronous function that is continuously called to set the uptime of the bot.
The function first stores the current time in a variable called currentTime. Then, it connects to the database named "economy" and finds the collection named "uptime".
Once found, the .updateOne function is called in order to set the element in the database called time to currentTime.

The previous example utilized just one Mongo function, .updateOne. The following example combines various functions together:

```javascript
async function replenishPower() {
    ...

    await ids.updateMany(
        { $expr: { $lt: ["$trailblaze_power", "$max_trailblaze_power"] } }, 
        { $inc: { trailblaze_power: 1 } }
    )
}
```

Here, a series of actions take place utilizing the **.updateMany** function. First, the expression checks if one element is less than another.
This is done with the **$expr** and **$lt** operators. If this is true, then all entries in the document that match this query have this element increased by 1.
By using **$expr**, we were able to create a conditional to execute the following command *only if* the conditional is true.

Both **setUptime()** and **replenishPower()** are events that are called periodically using [Cron](https://www.npmjs.com/package/cron), a popular node package.



Source: <a href="https://github.com/min-808/Seele/">Seele | Github</a>
