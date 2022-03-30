# Software Development with Teams

The best apps are made by large teams. But working with others, and especially coding with others can be really challenging. Often, the ability to work with others is a skill that is taken for granted or glossed over. There is often an expectation that people should just figure out how to do it on their own. But this doesn't have to be the case.

There is a separate discipline of project management that can take a lot of study and practice that teaches people how to manage projects and teams for the best results.

We're going to learn some basics about project management to assist you with your capstone project.

If we look at the diagram below, we have already begun the planning phase. Let's complete what we need to learn for planning and then learn about about the other phases and how we'll apply them to the capstone project.

![Agile Sprint Cycle](./assets/agile-sprint-cycle.png)

[Image Reference](https://www.workfront.com/project-management/methodologies/scrum/sprints)

## Background and Mindset

Building software comes with unique challenges, in particular: Continuous learning. Ideas and plans that seemed good/workable at the start often need to be adjusted as projects develop.

A lot of old management styles were not working for software development. Therefore, a new way of management came about that was called Agile in the early 2000s. Since then several variations have been created and each company will have their own systems, but generally, there are a few core principals that are always present.

[There are 12 core principles in the Agile Manifesto](https://www.agilealliance.org/agile101/12-principles-behind-the-agile-manifesto/)

Let's adapt and focus on a few of these for capstone:

- Early and continuous delivery of software (MVP)
  - Plan your app well enough that you deliver MVP as soon as possible
- Welcome changing requirements
  - As you build, different features may become unimportant and other features may end up becoming critical. Be open to adapting when needed
- Frequent delivery of working software
  - Rather than aiming for a large "complete" project on the final day of capstone, every day/week new working (small) features should be delivered by every teammate
- Projects require motivated individuals that are supported and trusted
  - Give each other the support and take time to build trust so that everyone can do their best every day
- The best way to convey information is face to face
  - Check in over zoom or in person\*
- Working software is the primary measure of progress
  - Take a moment to celebrate each victory and recognize your progress. There is always more to do, but don't let that take away from your team's progress.
- Sustainable progress, new features should be able to be added indefinitely
  - It should be possible to keep adding new features to your app. A new feature should not require a full rewrite of the app. Use best practices that you've learned in class to keep this possibility open. This will likely be one of the hardest thing to do as a team, it takes practice and a lot of learning from mistakes
- Maximizing the work not done is essential
  - Everyone wants to do a great job. It can feel like saying "yes" to all the ideas is the way to achieve greatness. But focusing on the the most critical features and learning to say "no" to distractions will help you build each component really well and give you a strong foundation to build on top of, if/when the time comes.
- Regular reflection and fine-tuning adapting behavior
  - Working on software and working on teams is hard. Each team will have a unique skill set and a unique work dynamic. Learning to work with your team takes time and effort. Keep adapting to make the most of your team's skills and abilities.

Zoom best practices:

- Turn your camera on, unless you are sick. If you will not be turning your camera on, inform your teammate(s)
- Keep the meetings short and on point
- But also, take a moment to check-in on how everyone is feeling/doing

## Planning

You should have already begun planning your app. Now it's time to formalize your planning.

## Trello

You will be using Trello. Trello is an app that helps organize the work of teams. Trello is made up of lists and cards. Cards should primarily be used to put individual user stories.

You will work in several sprints over the next few weeks. A sprint is a process of planning the work for a short period of time. At the end of each sprint, you will look at the work completed and the work not completed and make a new sprint (plan) that adapts to where your team and app is at.

You will work with 5 lists

- Design
  - This is where you should attach links to your Wireframes, ERDs and your brief description of your app - that way everyone can easily find these assets. Later, you'll put these details/assets in the README.md of your app
- Backlog
  - Start by putting all your user stories here
- To-Do
  - These are the user stories (features) your team will be building during the current sprint. These are agreed on by the entire team during planning.
- Doing
  - These are the user stories your team is currently (actively working on).
- Done
  - These are the completed user stories.

## User Stories => Trello Cards

Convert your user stories into Trello cards. You'll likely need to revise and refine your user stories. This is a normal part of the process.

**Acceptable User Stories/Cards**

- Create a landing page
- Get a list of grocery items (JSON, API call)
- A grocery item can be edited by the user through a form

These are specific features that should be easy to check whether the functionality is there or not. They are also small features that are possible to build withing a short period of time.

**User Stories/Cards that Need Improvement**

- Users
- Full CRUD on grocery items
- Submit button for Edit one grocery item

The first one is too vague. What does users mean? What kind of functionality? What does a successful implementation look like?

The second one is also vague - is that the front-end? Back-end? Both? How many user stories are in this one card? If this is front and back-end is this a reasonable amount of work for a short period of time?

The final one is too small a task and the feature functionality is unclear. Creating a button is very small and simple. Also, does it imply the ability to edit an item?

## Check-ins

Daily check-ins are often referred to as `Stand-ups` the idea is that if everyone would be required to stand, the meetings would be shorter and people would be more focused on the core goal(s) of the meeting.

Typically, the following questions are asked:

- What did you work on yesterday?
- Wha will you work on today?
- What blockers are in your way?

If there is a bigger issue to discuss ("I don't think we should build x feature any more, we should do y") - set a separate meeting time.

If someone is blocked because they are not sure what to work on, talk it out.

If someone is blocked because they are stuck with their code, figure out a plan to get unblocked:

- Talk it out with another group member after the meeting
- Do some pair programming
- Ask an instructor for guidance

A good idea is to screen-share the Trello board and move the cards as a group. This can help clarify the work that is happening with different members.

## Reviews (Stand Downs)

About once a week, you will hold a longer meeting (30-60 minutes) to go over the work that was done in more depth, review how the team is doing and make plans based on the progress that has been made.

This should be a safe space to allow people to be honest about how it's going and to find constructive ways to make things better.

Things to cover:

- Accomplishments (~5 minutes)
- The things that went well (~5 minutes)
- The things that didn't go well (~5 minutes)
- The things that can be done better (~10 minutes)
- Improving communication/adapting the use of Trello (~5 minutes)
- What is everyone working on next, updating the Trello board (~10 minutes)

The following roles should rotate for capstone:

- One person should run the meeting (ask the questions, make sure everyone answers), make sure that the group stays on topic and after the meeting, sets up follow up meetings, as needed
- One person should take notes
- One person should update the Trello board
- If there is a fourth member, they should watch the time and make sure the meeting does not run over.

Further tips:

- Keep it positive/constructive
- Don't make it personal/don't take it personally
- Allow everyone to speak without interruptions
- Stay on topic

## Retrospectives

At the end of the module, you will get a chance to reflect on the capstone project.

## Background Reading

[The Secret Startup That Saved the Worst Website in America](https://www.theatlantic.com/technology/archive/2015/07/the-secret-startup-saved-healthcare-gov-the-worst-website-in-america/397784/)

## References

- [What is Agile](https://www.workfront.com/project-management/methodologies/scrum/sprints)
- [Sprint Retrospective](https://plan.io/blog/sprint-retrospective/)
