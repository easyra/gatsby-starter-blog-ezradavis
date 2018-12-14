---
title: Labs8 Sprint Challenge Week-3
date: "2018-30-11T19:22:21+0000"
---

This blog post will summarize the individual accomplishments contributed by me during the second week of the Labs8 Developer Maps Project. I will also be going into the many challenges I faced this week as well as the functionality was was responsible of implementing for the week of 11/30/18.

## BackEnd Refactoring and Favorite Model

Most of my week was spent either refactoring code in the backend or hooking up some of the backend functions to the frontend.

My refactoring involved make sure data was consistent across denormalized data. I created functions that when triggered would delete all data related to a user if the user was deleted from the database. I also documented several of my functions so they are easier to work with.

My front end involved hooking up the favorite routes to the model. Features like being able to favorite posts as well as the hearts showing up when you open the model were my responsibility

### FrontEnd Tickets

####Ticket: 1

Date: 11/28/2018

Name: Ezra Davis

Link to PR(s) completed last working day:
https://github.com/Lambda-School-Labs/Labs8-DeveloperMap/pull/79

Date: 11/29/2018

####Ticket: 2

Name: Ezra Davis

Link to PR(s) completed last working day:
https://github.com/Lambda-School-Labs/Labs8-DeveloperMap/pull/84

Date: 11/29/2018

####Ticket: 3

Name: Ezra Davis

Link to PR(s) completed last working day:
https://github.com/Lambda-School-Labs/Labs8-DeveloperMap/pull/91

### BackEnd Tickets

####Ticket: 1

Date: 11/26/2018

Name: Ezra Davis

Link to PR(s) completed last working day: https://github.com/Lambda-School-Labs/Labs8-DeveloperMap/pull/51

https://trello.com/c/BgU1KUbg/9-backend
####Ticket: 2

Date: 11/26/2018

Name: Ezra Davis

Link to PR(s) completed last working day:
https://github.com/Lambda-School-Labs/Labs8-DeveloperMap/pull/54


####Ticket: 3

Date: 11/27/2018

Name: Ezra Davis

Link to PR(s) completed last working day:
https://github.com/Lambda-School-Labs/Labs8-DeveloperMap/pull/66


####Ticket: 4
Date: 11/28/2018

Name: Ezra Davis

Link to PR(s) completed last working day:
https://github.com/Lambda-School-Labs/Labs8-DeveloperMap/pull/73

####Ticket: 5

Date: 11/28/2018

Name: Ezra Davis

Link to PR(s) completed last working day:
https://github.com/Lambda-School-Labs/Labs8-DeveloperMap/pull/79




##Detailed Analysis Ticket: 2

This ticket mostly involved me hooking up Lauren’s favoriting endpoints to the frontend. The  company page now asking a user if they would like to favorite or unfavorite a company’s post. If they answer yes, then the job post will be added to the database under the signed in user’s favoritePosting JSON object. If they click the heart again, it will ask if the user wants to unfavorite the post and will then proceed to remove the user from the database. The client will also have access to the post ID’s the user has favorited and will indicate to the user whether or not the post has already been favorited or not. 

## Feature Complete

All of my group members were great to work with. Whenever something needed to be done, the best person for the job would always assign themselves the tasks. Everyone worked efficiently and did not waste any time at all. Whenever someone needed help another person would be there to work them through it.

Our challenges were really more of a rush for time than anything. We were really close to not finishing and the scheduling issue on thursday really threw us off. We also ran into bugs last second that we really didn't have time to fix. The CORS bug 30 minutes before we had to present was extremely stressful for everyone in the group and the sign up breaking last second was very unfortunate. But none of these issue were too bad, and all of those bugs seem to be fixed now. These kind of challenges are overcome by all of use working as a team and using each other's idea to make a better product.



#Proof
[Proof](https://docs.google.com/document/d/12DsgXzGmi04PLaqHgyKvPHsQXP3VL4pqh1Xop0nLjYY/edit?usp=sharing)
# Whiteboard 
[WhiteBoard](https://youtu.be/vrN-D5vyw9Q)
# Github Contributions
[Github Contributions](https://github.com/Lambda-School-Labs/Labs8-DeveloperMap/graphs/contributors)


