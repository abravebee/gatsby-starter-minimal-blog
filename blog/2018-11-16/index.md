Part 1 - Individual Accomplishments this Week
Paste a link to your whiteboard interview. You may keep this set to private and add your PM, but you are encouraged to set it to unlisted. (Weeks 2-4)


Paste your team’s github contribution graph here and indicate your Github Handle:

@abravebee. This is the least I've spent writing actual code in four months, but I learned a lot about auth0, and I'm growing a lot more comfortable with netlify.

Provide a paragraph (5-8 sentences) summarizing the work you did this week, the challenges you faced, the tools you used, and your accomplishments

Three-day weekends seem like a great idea in theory, but I find in practice lately that they really trip me up. I decided to take on Auth0 this week, having skipped it during back-end project week and assuming that the tutorial made by my cohort's section lead would be enough for me to grasp it. Although I did learn a lot from her tutorial, it turns out, like most things related to software development, this was more complicated than it seemed. I spent almost all of Tuesday's project time with this tutorial, and thinking about how to implement what I'd gleaned from it on our project. I ran into a snag that I discussed with my teammates, and ultimately decided to keep some notes of what I'd learned in a markdown file in our repo so that we could start with that the next day.

Patrick and I ended up spending all of Wednesday in Auth0 Purgatory, trying to glean as much info as we could from the docs and various tutorials to figure out why nothing was working or breaking consistently. While it was in some ways a soul-sucking experience, it felt good to really dive deep into a technology and try to figure it out. One thing that has bothered me about Lambda's breakneck speed and my own very busy schedule is that I don't often feel I have the time to get as familiar as I'd like with new technologies. It was nice to have someone to consistently bounce thoughts off of, as well, as I didn't do a lot of pair programming before this.

Our PM, Keith, ended up coming to the rescue with a tutorial I had dismissed earlier in the day. From that I think I learned how easy it is to get confused and overwhelmed by just how many different ways there are to approach a problem. I think in the future I'm going to work on either reading as many as I can, or at least sticking with a certain approach until I'm certain I'm stuck (and not just stressed out). Patrick bridged the gap in what we were missing after hours, so my plan was to go over the tutorial Keith sent and Patrick's fix to make sure I understand what happened.

Thursday, I had more technical difficulties than I usually like to shake a stick at, and we also spent a considerable amount of time as a group debugging some issues in github and trying to get our deployment back up. Please note: in addition to the issues we were facing with git, I was also receiving errors from my terminal, making it impossible for me to make commits, so I instead pair programmed with Patrick and Joseph while we were trying to fix what was blocking us from MVP.

Tasks Pulled
List the tasks you pulled this week, and provide a link to the successfully merged PR completing that task and the trello card for that task.  You must have at least one front end and one back end. The expected total is 6 with a minimum of 4.


Ticket 1: Auth0
Github: https://github.com/Lambda-School-Labs/Labs8-MealHelper/pull/42
Trello:
Ticket 2: Netlify fix
Github: https://github.com/Lambda-School-Labs/Labs8-MealHelper/pull/50
https://github.com/Lambda-School-Labs/Labs8-MealHelper/pull/51
https://github.com/Lambda-School-Labs/Labs8-MealHelper/pull/52
Trello
Ticket 3: Helped Joseph find missing files after branch purge
Github: https://github.com/Lambda-School-Labs/Labs8-MealHelper/pull/57
Trello


Detailed Analysis
Pick one of your tickets and provide a detailed analysis of the work you did.  This should be approximately ¼ page of text, and at least three screenshots.

The most work I did with code this week was working with the Auth0 login, learning tutorials the first day and trying to bring it all together with Patrick the next day. I had realized some things were missing when I got to the end of the tutorial I'd been studying, so I wrote up everything I'd learned from it on Tuesday with the intention of having a reference when I linked up with Patrick on Wednesday. I'll compare screenshots of these instructions with the final solution.

![auth0-tutorial](../../imgs/wk02-auth0-tut2)
![auth0-tutorial](../../imgs/wk02-auth0-tut3)
![auth0-solution](../../imgs/wk02-auth0-sol1)
![auth0-solution](../../imgs/wk02-auth0-sol2)

So the major missing pieces were, for me, the binding, the callback, and several of the WebAuth keys. My memory likes to lapse when it comes to syntax, so I still need to look into why so many tutorials used `.bind()` instead of more recent ES6 syntax. The callback was something that was briefly covered in the initial tutorial I had used, and something that was present in several other tutorials, but I think we had run into some issues with it since we hadn't initially set up a component with a loading message. There were some demos which included a different way of accessing/manipulating the location history that I knew we would end up switching for `this.props.history`, but wasn't exactly sure where we would need to implement it. This was a good lesson for me as far as translating not only between languages, but between tools, and a heads up that I need to learn more ways of approaching problems within the languages I'm most familiar with. 

The biggie, though, was the WebAuth keys. We were struggling to get the idToken to set on local storage and were trying to figure out how to access the email so we could store it to keep track of our users. We want to make sure they can only access their own meal journal entries and ingredients, and it didn't make any sense to use only the idToken. One approach that we had seen was decoding the idToken to get profile info, but we ended up learning that changing the scope from `openid` to `openid email profile` would allow us to access it without needing an additional jwtdecode package.

It was a hellish couple of days trying to figure it out, but this is one of those situations where I do feel like the struggle made me stronger. That said, I think Patrick and I both need to get better at reaching out for clarification sooner.


Part 2 - Milestone Reflections
As a part of your journal entry, write ¼ to ½ a page reflecting on your experiences working with a team to integrate several servers, pages, APIs, and services into one project. Describe how your pieces of the project interfaced with and integrated with your teammates.

Since we'll be needing to pull nutritional info from the USDA API and OpenWeatherAPI, we decided that Joseph and Haywood would work together on getting the info from the APIs pulled down and displayed, and that Patrick and I would work on implementing Auth0 to protect those routes. This seemed natural since Haywood has experience with one of the APIs, I have some experience with Auth0, and Patrick and Joseph have the most familiarity with our database.

We also ended up running into some major issues with our repo, and spent a few hours with Keith on Thursday trying to get it all sorted out. Although the trouble itself was frustrating, and the time we had to spend on it contributed to my being unable to meet the individual goals to my satisfaction this week, it was a good experience for me as far as recognizing the value of being on a well-balanced team. I felt myself stressing less about the deadlines for the next day and focusing more on solving the problem of the moment. While it's important to be cognizant of when things are due, I think being in the moment is crucial to effectively solve problems, and it's one aspect of this work (and of life) that I've really struggled with. It also gave me some confidence that I will be able to contribute to a team as much as I will be able to benefit from one.

As a group, provide links to evidence that:

Front and back end servers are connected
Users can create accounts and log in through the front end via OAuth
All APIs and services are connected and can be interacted with through the front end. A test message is acceptable to meet this requirement

Front End deployment: https://lambdamealhelper.netlify.com/
Back End deployment: https://labs8-meal-helper.herokuapp.com/users