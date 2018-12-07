---
date: "2018-11-30"
title: "Week Three"
category: "General"
---

## Part 1 - Individual Accomplishments this Week**
* Paste a link to your whiteboard interview. You may keep this set to private and add your PM, but you are encouraged to set it to unlisted. (Weeks 2-4)

_whiteboard video is processing_

I tried to emulate more of an actual whiteboard situation here. I did study Linked Lists and thought about palindromes beforehand... I figure in a real job interview situation I would be studying. I actually plan to study all of the whiteboard problems in the whiteboard repo (I saw there were a lot of videos on youtube for Linked List Palindromes but I tried to only watch stuff that was pure theory or just talked about what Linked Lists are because I was really lost when I first read the instructions). I'm surprised my solution was so close to the model solution and it makes me wonder about the other ways of doing it. I kind of hoped it wouldn't be the same so I could learn a little more.

* Paste your team's github contribution graph here and indicate your Github Handle:

[](https://i.ibb.co/zP4mZNR/contributions.png)
@abravebee

* Provide a paragraph (5-8 sentences) summarizing the work you did this week, the challenges you faced, the tools you used, and your accomplishments

I worked almost entirely on the Alarms page this week and learned just how rusty I was on React and Redux. I'm definitely seeing the value of doing Labs before CS! The biggest challenge was mainly remembering how to interact with Redux state and when to use component state vs reducer/global state. I also found myself leaning a little too hard on a previous assignment at one point and found that I was creating a component we didn't need, so I was able to switch my thinking and come up with a better solution for the current project. A fear I had while working through the first three months of Lambda was that I would struggle too much to build something new. This helped encourage me and reminded me that problem-solving is part of the fun of developing. I think it helped mediate some of my impostor syndrome and anxiety as well.

### Tasks Pulled
* List the tasks you pulled this week, and provide a link to the successfully merged PR completing that task and the trello card for that task.  You must have at least one front end and one back end. The expected total is 6 with a minimum of 4.

**Front End**
* Ticket 1
  - Github: https://github.com/Lambda-School-Labs/Labs8-MealHelper/pull/73
* Ticket 2
  - Github: https://github.com/Lambda-School-Labs/Labs8-MealHelper/pull/85
* Ticket 3
  - Github: https://github.com/Lambda-School-Labs/Labs8-MealHelper/pull/86

**Back End**
* Ticket 1
  - Github: https://github.com/Lambda-School-Labs/Labs8-MealHelper/pull/77

* Ticket 2
  - Github: https://github.com/Lambda-School-Labs/Labs8-MealHelper/pull/88

* Ticket 3
  - Github: https://github.com/Lambda-School-Labs/Labs8-MealHelper/pull/90/files


Detailed Analysis
Pick one of your tickets and provide a detailed analysis of the work you did.  This should be approximately ¼ page of text, and at least three screenshots.

I think I had the most fun with the adding alarms page. I had learned through our courses how to add resources one at a time, but the client requesting this project had a different thought about alarms: setting them every X amount of hours, for folks who suffer with hypoglycemia. So I thought the best way to add alarms would be in a batch, where the user chooses the first and last times of day that they'll be eating (such as their waking times, or breakfast and dinner times), and then choose how many hours should pass between each alarm, or meal.

[](https://i.ibb.co/FVyk8gT/addAlarm.png)

This `addAlarm` function was my baby! I'm not always great when working with numbers so this took a lot of figuring out. I spent a lot of time working it out on paper and in repl.it to make sure my math in the for loop made sense. I ended up needing to use military time for these calculations, so in the options I set for the drop downs, I made the values military time. Originally I didn't have the usual leading zeroes on the AM times, as javascript won't allow for numbers with leading zeroes, but I found out that iOS needed them in there. Since it was fine for them to work with strings, I added the leading zeroes back in and just changed it back to a number in the function.

[](https://i.ibb.co/NThKPHR/options.png)

(I hate how long that ended up being, but didn't want to spend time optimizing my code when I needed to just make sure it was working first)

Of course, changing it back to a number drops that leading zero, so I had to throw in a conditional to add that 0 back on. After that, I decided to map through the array of alarm times and send each one to the database. I had considered doing a bulk insert on the back-end so we wouldn't have to make so many calls, but since I want the ability to add single alarms as well (especially for iOS), it seemed better to handle that on the front-end.


Part 2 - Milestone Reflections
Put your response to the weekly question and a link to your team journal assignment here.


