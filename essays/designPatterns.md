---
layout: essay
type: essay
title: "Behind the Scenes of Websites"
# All dates must be YYYY-MM-DD format!
date: 2026-04-30
published: true
labels:
  - Design Patterns
---

<img width="300px" class="rounded float-start pe-4" src="../img/designPatterns/Abstract Pattern.jpg">

## A True Designer

I want to make a confession: when learning about design patterns in software engineering, I initially thought they had something to do with patterns that should be implemented on a website. Things like color theory, shapes, and overall designs that make your website more eye catching and pleasing to visitors of your site. Hopefully, I'm not the only one who thinks that, but for those who already know about design patterns, you can already tell that it is not the case. Diving deep into the topic and conducting a little research showed that my initial thoughts were way off, where it was more about the internal structure of the code and definitely not the actual design patterns for websites.

To ensure that we are all on the same page, design patterns in software development are `documented, reusable solutions to recurring problems in software design.` Design patterns are templates that can be used in many different situations.

Even if this is your first time hearing about design patterns, you probably have used it throughout your coding journey without ever realizing it!

## Common Design Patterns

Here is a brief list of the most common design patterns you have perhaps used before during your coding journey.

### Factory Pattern

A factory pattern uses factory functions to create new objects without you having to use the `new` keyword. To give you an analogy, think of, well, a factory making prebuilt gaming desktops. Without a factory, everytime a customer buys a prebuilt gaming desktop, engineers need to figure out what type of case they want to use, graphic card, CPU, and what not on the fly. With a factory, it can follow a set blueprint to ensure every prebuilt gaming desktop is built exactly the same way. It is useful when you need to create multiple smaller objects that share the same properties, and even create cleaner and more readable code.

### Observer Pattern

An observer pattern consists of 3 important parts, which include:
1. Observers: A list that stores all the functions or objects that want to be notified.
2. Subscribers/Unsubscribers: Methods that allow you to add or remove observers from that list.
3. Notify: A method that loops through the observers array and calls each one when a specific event occurs.

Think of it as a YouTube Channel where Youtubers have that notification bell icon that let's their subscribers (observers in this case) to click where they will get notified everytime a Youtuber uploads a new video. If a subscriber no longer wants to see the content from the YouTuber, they have the ability to unsubcribe where they will no longer receive any notifications, and content from that Youtuber will be ignored on the subscriber's page. This pattern is helpful when you have to keep things in sync with the other components of your website. For instance, having a create and edit form where the edit form must have existing data for it to edit something, then updating that into some data source like a database.

### Singleton Pattern

A singleton pattern ensures that a class has only one instance and provides a global point of access to that instance. It was hard coming up with an analogy with this one, so I asked ChatGPT for a basic analogy, and it provided a really good one. Imagine an office where every time an office worker wants to print something, they would buy a brand new printer, set it up, print one page, and then throw it away (or leave it sitting there). Obviously, this wastes money, space, and memory. With a singleton pattern, there is one shared printer where all employees just send their documents to that one printer. Everyone shares it, and you don't waste resources creating new ones.

There are many more patterns, but here are some of the common ones that we mostly use in our coding life.

## Implementing Patterns in Our Project

For those who don't know, a few ICS 314 students and I came together to build something for the UH Community. More specifically, a centralized bulletin board where students can create, see, like, and comment on other people's events. It is a way for the UH Community to see ongoing events through a centrialized hub without looking around campus for different types of events. Most likely, our project will have a lot of observer patterns where there are databases that need to be monitored for updated like and dislike counters, comment sections, and new/updated events. Since we are implementing an admin account, we will be showing signs of a proxy pattern in our project. Web admins have the ability to delete events entirely if users try to post events that are not within the University of Hawai'i code of conduct. Of course, we shouldn't give this ability to the users, otherwise everyone would delete events if they don't like it. Having this proxy, or middle man, helps regulate the webpage by providing admin tools to those with valid clearence and to restrict these tools to just ordinary users.

Overall, learning design patterns in software engineering was an interesting concept yet confusing at the same time as I slowly realize how it was more and more of the code itself instead of the actual website.