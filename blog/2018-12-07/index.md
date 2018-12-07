---
date: "2018-12"
title: "Week Four"
category: "General"
---

# Part 1 - Individual Accomplishments this Week
* Paste a link to your whiteboard interview. You may keep this set to private and add your PM, but you are encouraged to set it to unlisted. (Weeks 2-4)
**Spiral Matrix Copy: https://youtu.be/cKRDWqByy4g .**

* Paste your team’s github contribution graph here and indicate your Github Handle:
[abravebee contributions](https://imgur.com/TVy8Er1)

**You know who it is! a brave bee! labs 8! 2018! let's do this...**

* Provide a paragraph (5-8 sentences) summarizing the work you did this week, the challenges you faced, the tools you used, and your accomplishments.

**I was unfortunately unwell this week and therefore unable to put in as much work as I would have liked. I actually still feel horribly unwell even now and I hate that I have to rush through this dev journal but oh well, I guess it's good practice for the future. Anyway, I think I'm one of the few people who actually likes working with CSS, so I'd been looking forward to spending all week on it. Unfortunately (there always seems to be an unfortunately, and this is the second one in four sentences, yikes), we all realized/discovered that much of our code is/was such a hot mess that we needed to make adjustments to it before working on the CSS. We rediscovered that this problem was even more of a tangle than we thought half-way through the week. I suppose we learned a lot from it, but I'm hoping I get to spend much more time making things pretty next week.**

## Tasks Pulled
* List the tasks you pulled this week, and provide a link to the successfully merged PR completing that task and the trello card for that task.  You must have at least one front end and one back end. The expected total is 6 with a minimum of 4.

* Front End

https://github.com/Lambda-School-Labs/Labs8-MealHelper/pull/115

https://github.com/Lambda-School-Labs/Labs8-MealHelper/pull/130

https://github.com/Lambda-School-Labs/Labs8-MealHelper/pull/137

https://github.com/Lambda-School-Labs/Labs8-MealHelper/pull/151


* Back End

**The back end is pretty much done. I think the only work done on it this week was putting routes back in that were accidentally deleted in merges, but we're not deploying the master branch on heroku (it has its own branch) so PRs aren't required for those little fixes.**

## Detailed Analysis
* Pick one of your tickets and provide a detailed analysis of the work you did.  This should be approximately ¼ page of text, and at least three screenshots.

**I spent most of my time in alarms again this week, but I had a lot of fun! I had originally used `react-select` for my drop-down menus on the alarm adds, but since I was having so much trouble styling them and the boys had used `reactstrap` on the other pages, it seemed better to change over to that, so I did!**

[dropdowns in reactstrap](https://imgur.com/NYu7i3g)

**And this meant refactoring the way I was grabbing values and sending them to state.**

[new functions for new dropdowns](https://imgur.com/QXatlJg)

**The one drawback to the styling is that `reactstrap` apparently uses a lot of !important tags in their library, so you have to use !important tags to override them in your own code. I hate having to use such heavy specificity but at least it worked, whereas even copy-pasting code straight from `react-select`'s documentation wasn't having the expected effect.**

[ugly !importants](https://imgur.com/WaW3vrn)

**I also had some trouble with the custom modal I had built. Never did finish that out since it worked just fine on my Notes project, but once again, I went with the consistency of using a `reactstrap` modal as done with our logout function.**

[a new modal](https://imgur.com/tyckxqS)

**In general, I'm not really a huge fan of libraries like this, and only used them due to the time crunch. I'd like to get much more practice building things like modals and dropdowns from scratch so I can have more control over them.**

# Part 2 - Milestone Reflections
* As a part of your journal entry, write ¼ to ½ a page reflecting on your experiences working with a team to make your product look and feel as good as it works under the hood. Describe how the duties of you and your team shifted tasks shifted towards the front end - and debugging the back end to improve UX.

* As a group, provide documentation of your progress and remaining tasks

* Link to each page and describe any remaining bugs, fixes, or tasks that need to be completed on that page

**Okay, so let's be completely honest here. I was pretty frustrated this week. Between being sick, and realizing just the extent of the mess in much of the app, I was having a hard time not becoming angry. I had tried in the beginning of labs to start setting up boilerplate that would keep us from running into too much spaghetti code and give us some consistency to work with. But I think that was kind of ignored pretty early on as we were all rushing through to make sure we were meeting MVP each week.**

**The thing is, while I think we were all earnest in our thoughts that we'd be able to go back and fix things up later, I don't think we did this soon enough. I really think we should have been fixing everything up before making the PRs. It's one thing to slapdash it together long enough to make sure you have the right idea about functionality. But it seems like we built a lot of files and components that were never used because where we would normally import those things, everything ended up just being written directly. I imagine this was a combination of rushing due to deadline stress, and working when not adequately fueled by either sleep or food (I think all three of us webdev people were probably guilty of this at some point).**

**I don't mean to deflect or cast blame at all. I just think/hope we've all learned a really important lesson here about cleaning up as you go, communicating consistently, and not pushing ourselves to the limits of what our brains/bodies can handle. And I'm trying not to cry at the thought of our upcoming code review and how much we need to refactor before then. But whatever!!! It's all good!!! Stay positive!!!**