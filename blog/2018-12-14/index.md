---
date: "2018-12-14"
title: "Week Five"
category: "General"
---

# Part 1 - Individual Accomplishments this Week

* Paste your team’s github contribution graph here and indicate your Github Handle:
![abravebee contributions]()

**abravebee**

* Provide a paragraph (5-8 sentences) summarizing the work you did this week, the challenges you faced, the tools you used, and your accomplishments.

**I'm so tired I barely remember what happened this week. We ran into a bunch of issues with structure when we started working on the UI, so tons of things ended up non-functional last week and having to be refactored this week. I spent a lot of time updating the landing page initially because I didn't realize just how much functionality we had lost (or how much we still needed to implement). I did manage to get the meal list and single meal view up and looking nice, but I had trouble with displaying nutrients in the mealbook and with updating meals. This seems like a residual lesson about the importance of keeping code neat, and maybe about making sure the goals of the app/UX are crystal clear as soon as possible.**

## Tasks Pulled
* List the tasks you pulled this week, and provide a link to the successfully merged PR completing that task and the trello card for that task.  You must have at least one front end and one back end. The expected total is 6 with a minimum of 4.

* Front End
https://github.com/Lambda-School-Labs/Labs8-MealHelper/pull/202

https://github.com/Lambda-School-Labs/Labs8-MealHelper/pull/191

https://github.com/Lambda-School-Labs/Labs8-MealHelper/pull/186

https://github.com/Lambda-School-Labs/Labs8-MealHelper/pull/175

https://github.com/Lambda-School-Labs/Labs8-MealHelper/pull/165

* Back End

**Same story as last week, most back-end work was just tweaking.**

## Detailed Analysis
* Pick one of your tickets and provide a detailed analysis of the work you did.  This should be approximately ¼ page of text, and at least three screenshots.

**It's one of the least important things involving the app, but I'm actually really proud of my work on the landing page! I spent a lot of time re-organizing its html structure so I could use flexbox more effectively.**

![]()

**I really enjoy the UI/UX side of things but I think I need more practice because I ended up keeping negative margins on a lot of elements on the landing page, which I understand is bad practice. I think I probably would've been able to figure this out given a little more time, but I was refactoring someone else's code and that's how they'd gotten it to work. It didn't seem smart to spend too much time completely refactoring everything under the time crunch.**

![]()

**Building the meal list and single meal views were more complicated than I expected, too. Particularly grabbing the nutrient information. A nested axios call worked well enough on the single view, but triggered an infinite loop in the list view. I know this has to do with my lifecycle methods but I struggled to figure out how to get around this, and it was unfortunately a late-night problem, so I still haven't worked it out. I definitely need to refresh on my React/Redux understanding particularly when it comes to the lifecycle methods.**

![]()

![]()

****

# Part 2 - Milestone Reflections
* As a part of your journal entry, write ¼ to ½ a page reflecting on your experiences working with a team to bring an application to completion. The 90-90 rule is a quip referencing the very real difficulty of truly completing a project. Describe some of the final tasks that were the most difficult for your team to resolve - challenging bugs, layout and presentation woes, or anything else that was easy to get mostly working, but hard to get perfect

**I think it all mainly came down to having to clean up all the things we rushed through when it got down to UI. We definitely should've had a clearer vision of layout and should have been much more careful about checking structure before merging things in. We started out trying to grow our front-end with the back-end as was recommended, but I think we let deadline anxiety get the best of us and allowed ourselves to get away with too much messiness. In general, most of our basic communication with the back-end works, but I personally think our UX leaves a lot to be desired. I could work for weeks on that alone. I hope as I continue to practice and grow as a developer, I get better at working under the deadline pressure and am able to stay organized. I particularly look forward to working in an environment where the organization has already been established, and I simply have to follow it. I think that'll end up making things a lot easier to deal with. But I've learned a lot about how to approach building side-projects, as well. While things didn't go as well as I had initially hoped, I think I really learned a lot of valuable things not only about web development, but about working with a team, and my own strengths and weaknesses as a developer.**