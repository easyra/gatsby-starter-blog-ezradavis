---
title: Labs8 Sprint Challenge Week-1
date: "2018-11-11T19:22:21+0000"
---

This will be a summary of the individual accomplishments I have contributed to during the first week of the Labs8 Developer Maps Project. This blog post will be going over the many responsiblities and challenges I needed to overcome in order to work complete the necessary requirements for the week of 11/9/2018.

## Server initialization and Firebase Data Structure

My primary responsibilities during the project involved dealing with and setting up the project's backend server. Much of my time spent during the first week was spent understanding the optimal ways to structure my data in Firebase's Realtime Database. Firebase's Realtime database is a NoSQL database which stores all of its data in a JSON Object. 

This was a major challenge consider I had never had experience with this type of database before and had to figure out how to structure my information in a way where I could access it without being able to rely on the complex querying functionality I had taken for granted in my time working with Relational Database Management Systems like SQLite. 

Once I tackled this problem, my next step was hooking our Firebase Realtime Database to our projects Node js backend as well as setting up the majority of its routes. Some objectives such as hooking up the Realtime Database to our Node js backend and setting up GET routes were pretty straight forward and did not take long once I had finished reading the docs. Routes involving updating the database however, weren't as easy and required reviewing my learning resources for Firebase multiple times.


### FrontEnd Tickets

####Ticket: 1

Date: 11/8/2018

Name: Ezra Davis

Link to PR(s) completed last working day: 
https://github.com/Lambda-School-Labs/Labs8-DeveloperMap/pull/20

### BackEnd Tickets

####Ticket: 1

Date: 11/6/2018

Name: Ezra Davis

Link to PR(s) completed last working day: https://github.com/Lambda-School-Labs/Labs8-DeveloperMap/pull/4

####Ticket: 2

Date: 11/7/2018

Name: Ezra Davis

Link to PR(s) completed last working day: 
https://github.com/Lambda-School-Labs/Labs8-DeveloperMap/pull/7

Link to Trello card(s) completed last working day: 
https://trello.com/c/BgU1KUbg/9-backend

####Ticket: 3

Date: 11/8/2018

Name: Ezra Davis

Link to PR(s) completed last working day: 
https://github.com/Lambda-School-Labs/Labs8-DeveloperMap/pull/13

Link to Trello card(s) completed last working day: 
https://trello.com/c/3AYIdrAj/27-signin-and-signup-modal

Link to Trello card(s) being worked on...current day: 
https://trello.com/c/x5ndYqcg/11-deployed-to-the-web

##Detailed Analysis Ticket: 3

This ticket was easily the most difficult part of my week. Implementing the functionality required to complete my ticket challenged both my understanding of data structuring and data constituency in a NoSQL database. 

As I began righting my CRUD endpoints, I notice how complicated and counterintuitive I would have had to make my data queries if I wanted to pass important information to my client. As I began looking more and more at the functions I had already written at this point, I realized that I was structuring my data and my functions like I was working SQLite. I needed to start denormalize my data structure, and make it so that i could retrieve data via simpler and more efficient queries. 

When I realized the problem I did a complete overhaul of how our data was structured. Data that I would try and retrieve via complicated queries matching certain types of data with each other, was converted into much simpler duplications of already existing data. This then made the route making portion of the project significantly more Sharif forward. GET's involving companies and employers were significantly easier to make and as well as send to the client. I was now much closer to getting our project to a clear, intuitive, and well-structured data structure and Node js app. My next challenge was making sure my data was consistent whenever I need to update or post new information.

Data consistency is always a challenge in a NoSQL Database. In SQLite I was always used to normalizing my data. So if I need to update something, it would always be in the same spot. In a NoSQL Database however, a developer could have multiple duplications of the same data in order to simplify queries. And as a developer myself, I need to make sure my data remained consistent whenever the client would request a POST or a PUT. Firebase does this by sending an object filled with the path names to the data that needs to be updated and the value the path name is being updated with. That way, I can update multiple points of data through a single function. And this is done atomically as well, which means I'm safe from any sort of error on the client end leaving my update incomplete. 

* [Deployed FrontEnd](https://clever-liskov-29b49a.netlify.com/)
* [Deployed BackEnd:](https://intense-stream-29923.herokuapp.com/api/database/seekers)
* [User SignIn](https://cdn.discordapp.com/attachments/508055941145690142/510520021609480192/Week1SignInShow.PNG)
* [User Register](https://cdn.discordapp.com/attachments/508055941145690142/510520026097254420/Week1SignInshow2.PNG)
* [FrontEnd Screenshot](https://cdn.discordapp.com/attachments/508055941145690142/510519407634546688/Capture.PNG)
* [Realtime Database](https://cdn.discordapp.com/attachments/508060338944606214/510527647315656711/unknown.png)
* [Authentication DataBase](https://cdn.discordapp.com/attachments/508060338944606214/510527754106830879/unknown.png)
