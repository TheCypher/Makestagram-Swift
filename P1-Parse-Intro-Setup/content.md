---
title: "Setting up Parse"
slug: setting-up-parse
---

To build a photo sharing app we will need to exchange information between multiple users on multiple devices.

In the *Make School Notes* tutorial we built an app that only stores information locally on the user's phone. There is no way of sharing information with other users or accessing notes from other devices. This is fine for some apps; however, most applications need to provide a way for multiple users to to interact with each other. In such cases we need to store the information used in the app on a server that is accessible by all users.

#What Does Parse Do for Us?

Until a few years ago, it was necessary to write an entire server application to handle the server side code of your app - now we can use the Parse platform instead. Parse allows us to define the different types of objects we want to store in our application, as well as the relationships between them.

Additionally Parse provides an iOS library. This makes it easy to interact with the Parse server from within our app.

We have prepared a brief lecture that will introduce you to the core concepts of the Parse framework:

<iframe width="560" height="315" src="https://www.youtube.com/embed/q8NW_FrwQ5A" frameborder="0" allowfullscreen></iframe>

You can download the slides [here](https://s3.amazonaws.com/mgwu-misc/SA2015/LectureSlides/ParseIntro.pdf).

Throughout this tutorial you will get to know Parse in detail. Our very first step is setting up a Parse account and setting up our first app.

#Setting up a Parse Account

First, sign up for an account.

> [action]
Go to [Parse.com](http://parse.com). Enter your email address, choose a password, and name your app *Makestagram*.
![image](signup_parse.png)


Now you have created your first Parse app!

On the next screen you will see a bunch of services that Parse provides. We will only be using the *Core* product which allows us to create a data model for our application.

> [action]
Select *Core* in the top bar to open the Parse Data Browser:
![image](parse_core.png)

This is the place where we can see and edit the data model for our application. Before we dive into the details of how to create new classes, we should discuss what the data model for *Makestagram* should look like.
