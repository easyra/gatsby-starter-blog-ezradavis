---
title: Labs8 Sprint Challenge Week-4
date: "2018-712T19:22:21+0000"
---

This blog post will summarize the individual accomplishments contributed by me during the second week of the Labs8 Developer Maps Project. I will also be going into the many challenges I faced this week as well as the functionality was was responsible of implementing for the week of 12/7/18.

## Bug Fixes

Most of my week was spent fixing several bugs in the program. This week’s efforts were spent improving the frontend, so most things on the backend where already taken care of. Backend refactoring, hooking new GETs to the frontend,and fixing crashes involving the favorites and company profile page where my main responsibilities for this week.


### FrontEnd Tickets

####Ticket: 1

Date: 11/28/2018

Name: Ezra Davis

Link to PR(s) completed last working day:
https://github.com/Lambda-School-Labs/Labs8-DeveloperMap/pull/110

Date: 11/29/2018

####Ticket: 2

Name: Ezra Davis

Link to PR(s) completed last working day:
https://github.com/Lambda-School-Labs/Labs8-DeveloperMap/pull/113

Date: 11/29/2018

####Ticket: 3

Name: Ezra Davis

Link to PR(s) completed last working day:
https://github.com/Lambda-School-Labs/Labs8-DeveloperMap/pull/118

### BackEnd Tickets

####Ticket: 1

Date: 11/26/2018

Name: Ezra Davis

Link to PR(s) completed last working day: https://github.com/Lambda-School-Labs/Labs8-DeveloperMap/pull/103

https://trello.com/c/BgU1KUbg/9-backend
####Ticket: 2

Date: 11/26/2018

Name: Ezra Davis

Link to PR(s) completed last working day:
https://github.com/Lambda-School-Labs/Labs8-DeveloperMap/pull/125


####Ticket: 3

Date: 11/27/2018

Name: Ezra Davis

Link to PR(s) completed last working day:
https://github.com/Lambda-School-Labs/Labs8-DeveloperMap/pull/110




##Detailed Analysis Ticket: #110

The tasks in this ticket had to do with hooking up the new back end functions from the previous day with the front end. The main reason for this is to reduce axios calls. Right now we have a lot of unnecessary axios calls being made that could be alleviated with a backend that takes the needs of the frontend into more account during its design. 

One of the backend functions was just a combination of two data querying. The first being the job postings and the second being the jobs the user signed in has favorited. I also created fi else statements to control which axios calls get made. For example if the user isn’t signed in, the react app wont query for a list of favorited jobs. But if the user something signs in after the component mounts(which seems to happen on refresh), it will query favorited jobs for the that user. 

The second function was a PUT that was suppose to replace the DELETE and POST for managing what was in the user’s favorites page. Originally whenever you clicked on the heart, it would pop up and alert that would ask you if you wanted to delete or add the favorite followed by a axios call depending on the choice. This means every time someone added something or removed something, it would be making a call to the server. The function was also sending the entire job object through the server as well on post. This was obvious not a great solution to favorite considering how slow it would be. So now what the component does is send a list of all the favorited job post keys that are in state after the user decides what he wants to favorite, and the backend populated the users favorites page based on the keys sent. 

##Presentation

I didn’t personally feel much of a shift during the 4th week. I’ve pretty much always been debugging for refactoring the backend to fit the client’s needs. I did get to work a lot more with front end when I was hooking up my backend functions to the front end, and I think that was important because it let me know what I needed to do in the future to improve my backend skills. But other than that, not much different than the rest of the week for me. Someone on team was able to write function with firebase and gain some more experience in the process.

[Proof](https://docs.google.com/document/d/1ZCGal4wJqT8iXlERnLJ_JnME_vf0X2kmlaEnTM1Eakg/edit)
[Whiteboard](https://youtu.be/5gV3AHWMuYU)
[Github Contributions](https://github.com/Lambda-School-Labs/Labs8-DeveloperMap/graphs/contributors)


