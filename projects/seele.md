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

Seele is a Discord bot I spent Winter 2023 working on. This project helped me learn about Javascript, as well as how to structure a database schema.

Seele is implemented using [Discord.JS](https://discord.js.org/), a Node.js module that interacts with the Discord API seamlessly. Within three weeks, I created a fully-fledged bot that has an economy system, various games, and daily login rewards.

In this project I gained experience with [MongoDB](http://mongodb.com) for database storage, Mongoose for creating a connection between MongoDB and the Node.js runtime environment, and Javascript for creating the interactions.

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
This is done with the **$expr** and **$lt** operators. If this is true, then the selected element is increased by 1.
By using **$expr**, we were able to create a conditional to execute the following command *only if* the conditional is true.

Both **setUptime()** and **replenishPower()** are events that are called periodically using [Cron](https://www.npmjs.com/package/cron), a popular node package.



Source: <a href="https://github.com/min-808/Seele/">Seele</a>
