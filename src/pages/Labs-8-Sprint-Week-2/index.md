---
title: Labs8 Sprint Challenge Week-2
date: "2018-11-11T19:22:21+0000"
---

This blog post will summarize the individual accomplishments contributed by me during the second week of the Labs8 Developer Maps Project. I will also be going into the many challenges I faced this week as well as the functionality was was responsible of implementing for the week of 11/12/12.

## BackEnd Refactoring and Admin SDK Support

Most of my week was spent optimizing and refactoring the backEnd. Many of our route were set up to be functional enough to get the job done. I tried to make them even better.

Many of our routes were set up to support atomic multi-path updating. That way our data would always be consistent if there were some kind of error on the client or server. The folder structure for our backend was also restructured so that it's both easier for people working primarily in the frontend or backend to work on. The code for our routers were also broken up into two separate files so that it is easy to read as well as find required routes related to a job seeker or a company.

We also replaced the regular firebase SDK with the Firebase Admin SDK. The Admin SDK gives us access to certain functionalities that allows for easier development. One example is the Admin SDK's ability to let us ignore firebase database rules. Previously we were afraid to write any rules for our database that would control for unformatted data, because we thought it would make development much slower. But now that we have the Admin SDK, something like this wouldn't be a problem.

### FrontEnd Tickets

####Ticket: 1

Date: 11/15/2018

Name: Ezra Davis

Link to PR(s) completed last working day:
https://github.com/Lambda-School-Labs/Labs8-DeveloperMap/pull/38

### BackEnd Tickets

####Ticket: 1

Date: 11/13/2018

Name: Ezra Davis

Link to PR(s) completed last working day: https://github.com/Lambda-School-Labs/Labs8-DeveloperMap/pull/24

####Ticket: 2

Date: 11/15/2018

Name: Ezra Davis

Link to PR(s) completed last working day:
https://github.com/Lambda-School-Labs/Labs8-DeveloperMap/pull/33


####Ticket: 3

Date: 11/8/2018

Name: Ezra Davis

Link to PR(s) completed last working day:
https://github.com/Lambda-School-Labs/Labs8-DeveloperMap/pull/35


##Detailed Analysis Ticket: 3

I'll be talking about this ticket because it was personally a lot of fun for me. This was the ticket where I implemented Cloud function, and today I'll be talking about some challenges and hang ups I had during this time.

Cloud functions are functions that get triggered based on certain events from our firebase server. This concept was really fascinating to me since I had only really seen functions triggered on the backend via requests from a client. The idea that I could functions activated whenever a user is added or deleted and this can been written completely independent from my node js server was really interesting and opened our project up to a lot of options.

I initialized the firebase functions using the Firebase CLC and implemented two functions. The first one is an OnDelete connected to our authentication server. This function will activate whenever a user is deleted from the the authentication server and automatically deleted all of the users related data in the database. This function is meant to help with data consistency and remove useless data from our database. The second one is a function that sends an email using nodemailer to anyone who signs up to our website. This one isn't as functional yet due to restricted from google's email services. once that's sorted out though it should be good to go.

