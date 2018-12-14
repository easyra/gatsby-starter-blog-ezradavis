---
title: Labs8 Sprint Challenge Week-5
date: "2018-14-12T19:22:21+0000"
---

This blog post will summarize the individual accomplishments contributed by me during the second week of the Labs8 Developer Maps Project. I will also be going into the many challenges I faced this week as well as the functionality was was responsible of implementing for the week of 12/14/18.

## BugFixs and BugFixs

My week was pretty light. Mostly just fixing bugs. One bug I fixed involved the favorite page not working if you didn’t have any posts. A similar bug was also in the page where companies can add jobs. If the company didn’t have any posts. They couldn’t add anymore without the page breaking. That bug in particular was really hard to figure because even though it was similar to the bug in the favorites modal, it was really hard to tell what was happening due to the constant page refreshes set up. I also worked on hooking up the modals that tell the user whether or not the client is loading data from the node js server.

### FrontEnd Tickets

####Ticket: 1

Date: 11/28/2018

Name: Ezra Davis

Link to PR(s) completed last working day:
https://github.com/Lambda-School-Labs/Labs8-DeveloperMap/pull/140

Date: 11/29/2018

####Ticket: 2

Name: Ezra Davis

Link to PR(s) completed last working day:
https://github.com/Lambda-School-Labs/Labs8-DeveloperMap/pull/142

Date: 11/29/2018

####Ticket: 3

Name: Ezra Davis

Link to PR(s) completed last working day:
https://github.com/Lambda-School-Labs/Labs8-DeveloperMap/pull/143

####Ticket: 4

Name: Ezra Davis

Link to PR(s) completed last working day:
https://github.com/Lambda-School-Labs/Labs8-DeveloperMap/pull/145

####Ticket: 5

Name: Ezra Davis

Link to PR(s) completed last working day:
https://github.com/Lambda-School-Labs/Labs8-DeveloperMap/pull/146

### BackEnd Tickets

####Ticket: 1

Date: 11/26/2018

Name: Ezra Davis

Link to PR(s) completed last working day: https://github.com/Lambda-School-Labs/Labs8-DeveloperMap/pull/132

https://trello.com/c/BgU1KUbg/9-backend




##Detailed Analysis Ticket: 2

For my detailed analysis, I’ve decided to talk about making how I updated my auth middleware to make it automatically assign a profile picture to the user upon creation. The change was pretty simple and the code for it wasn’t very large. Basically this is how it works. Whenever a user is create, if they sign into a google or github account that has a profile picture, firebase auth will store it in there database. So what my auth middleware does is grab the profile picture from the auth server so that it can be stored in the req.body object. If the user doesn’t have a profile picture in auth, the user is given a default profile picture.

## Polish

Working on our Labs 8 project has been pretty fun through and through. Getting the opportunity to build a full fledged app and working with such a friendly team has been one of the best experiences I’ve had at Lambda. 

The first two week were probably the most difficult. We were using a FERN Stack, so I had to learning firebase pretty much by myself. The first couple weeks, I wasn’t really able to code all that much and a lot of my time was spent just reading and watching firebase videos. Once I got a handle on it though, it was pretty straight forward from there.  

Mappajob is a web application designed to help employers in need of employees and employees in need of jobs find each other via geolocation. Our application is built with a FERN stack which means Firebase, Express, React, and Node js. Any company can sign onto our app, after paying a fee, can post up to 5 jobs. These jobs show up on the company’s page, and a job seeker can see this page and click the link on the page to apply for a job. 

#Proof
[Proof](https://docs.google.com/document/d/12DsgXzGmi04PLaqHgyKvPHsQXP3VL4pqh1Xop0nLjYY/edit?usp=sharing)
# Whiteboard 
[WhiteBoard](https://youtu.be/vrN-D5vyw9Q)
# Github Contributions
[Github Contributions](https://github.com/Lambda-School-Labs/Labs8-DeveloperMap/graphs/contributors)


