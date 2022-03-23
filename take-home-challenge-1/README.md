# Take Home Challenge 1

Take home challenges are a great way to show off your coding skills. Many times, you'll be asked to code something that you have not done before, or to use a technology you have not had time to learn yet. It is a great opportunity to level up your skill level and learn more about how different developers work at their companies.

Regardless of the outcome, take home challenges are opportunities to broaden your understanding of the tech field and refine your abilities.

## What are Take Home Challenges

Take home challenges are ways to gauge your coding ability by giving you a mini-project or a more complex algorithm to solve on your own time.

After you work on it, you will submit your work and then you will likely get a follow up interview to talk through your project. You also may be asked to continue to build out a feature with someone from the company, so they can learn more about how you work with others.

Take home challenges are very broad, from just doing CSS, do building an API, to a full stack app, to making a game, nearly anything is possible. You may or may not be able to choose the language you code in and may or may not have a choice about the tech stack (MERN, Ruby on Rails, Django etc.).

Take home challenges often have an estimated time for completion. Usually anywhere between 2-8 hours. Sometimes they will time you (send you the challenge at 10am and expect a submission by 2pm) and sometimes they will tell you to work on it over the span of 2 - 7 days.

## Ending an Interview Process

You have the right to say no. If the challenge unreasonable, for example: It is expected to take 2 weeks of full-time work, if they expect you to pay money to take some sort of test, if the take-home is on cyber security and that is not your interest/doesn't match the job description, you can say no. Politely tell them you are not interested in continuing and then the interview process will be over. Remember, the interview process goes both ways. Not only are they interviewing you to be a good fit, you are interviewing them to see if you would fit in with them. Walking away from an interview can be a tough choice, but you must set your best interests first.

## Expectations

Even though the code challenges gives an estimated time, if they are not setting a strict time block, it will likely take you longer. Estimating how long a project will take is difficult, both for the people administering the take home challenge and for the people taking them.

Usually, there are some minimum expectations. Doing the bare minimum is usually not enough in a competitive job market. Most take home challenges will list bonuses or other things they are looking for (clean code, responsive design).

However, you don't want to overdo it. If the challenges is supposed to take 4 hours, but you spend 40 hours on it, that typically doesn't go over well either.

As we go through more tips and tricks, you will get a clearer picture. Additionally, we will give you some practice take-home challenges so that you get a better idea of what they are like. With these practice challenges, you can talk to your instructor about expectations and clarify whether you have the right approach.

## Getting Started

### Read and Understand the Prompt

The first thing you want to do when you get a take-home challenge is to read all of the instructions, carefully.

Take notes, make bullet points, write down any questions you have.

Take home challenges are not only checking for your ability to code, but also check how well you follow instructions, how well you work on your own and possibly, how you ask for help/clarifications.

For example, you may be asked to build a weather app. But it doesn't say if you should use React, Vue, or vanilla JavaScript. It's good to get clarification if there is an expectation (or preference) to build with a certain technology.

### Plan

Take the time to create wireframes and user stories.

Don't plan or add extra features. It may be cool to add Google maps, but if it is not asked for, do not do it.

If it is unclear, for example, when building a weather app, whether the app should work with a zip code or city name, you can ask for clarification.

Figure out the order of what you are going to build and then estimate the time you think it should take.

### Build a Hello World App

It is tempting to jump in and build everything at once. Slow down and build a very simple app and make sure it is set up correctly.

This is even more important if you are working with a language or tech you are less/not familiar with.

- Use git/GitHub as they recommend
- Set up the configuration
  - Create a `README.md` and write down the instructions on how to get your app up and running if they will be testing it locally. Think back to your past labs or tutorials you've take where the set up instructions were missing or unclear. The compare it to a lab or tutorial that had clear instructions. You can reference one with good instructions to help guide you.
  - Things like running `npm i` should not be taken for granted, write out each step required, like a very simple recipe to follow
  - If a `.env` file is required, be sure to include steps for that and what the environmental variables should be
- If it is supposed to be deployed online do that first
- If they want it sent as a zipfile, figure out how to zip and unzip the files

Do not forget to `git add` and `git commit` once the basic app is working. Be sure to write descriptive commit messages.

Be sure to `add` and `commit` often. Use branches when adding new features or if you realize you need to refactor the code.

### Build the Rest of the App

You should build your app in this order:

1. Make it work - all basic required functionality
1. Make your code pretty

- Go back and proofread your code and make sure you fix indentation
- Improve your comments, improve your variable names etc.,
- Use the same version of syntax (if you use `const`/`let`, don't sometimes use `var`, declare your functions in the same way (unless you have a specific reason not to in a couple places) etc.))\*

1. Make your app pretty (fix CSS, style forms, make it responsive, use a neutral/modern color theme, use a simple modern font (even the `sans-serif` built-in default can make an app look much more modern))\*\*
1. Make it work even better (fix bugs, handle edge cases, handle errors)

\* If you struggle with indentation and consistent code formatting, consider installing a linter/code formatter like `prettier`, adjust the settings so that it will automatically format your code for you on save.

\*\* If this is a front-end focused challenge that comes with a specific mockup to match, be sure to spend more time matching the mock-up. Be sure to use the provided fonts and colors and any other provided specifications.

**Bonus** - if it is an option, use tests/implement TDD. We have not yet covered it in class, but you should take some time to learn on your own. Especially if you know the company uses tests/TDD or if they have it as a stretch/bonus feature. You can look back at previous labs that had testing for examples.

**Bonus** - make it fast. This is typically not necessary for a JR level position, but if you can find ways to make the app faster, it is recommended. As you progress as a developer, this optimization should be something you definitely take into deeper consideration.

### Common Mistakes

- Not managing your time well and scope creep
  - Make sure you stick to your plan. If you are going over time, try to understand if it is because you are stuck or if you are trying to do too much
  - Maybe you thought you would add a cool CSS animation that was not asked for, and suddenly you have spent 3 hours trying to get it to work
- Don't try to learn too many things at once
  - If the app is supposed to be built in React, this is not the time to experiment with redux, mobx, graphql, formik etc. all voluntarily at the same time. Stick to the basics, perhaps try one simple-ish new thing.
  - If the app already requires you to learn new tech, don't try to learn even more new tech, stick to the bare minimum new things
- Make too many assumptions
  - If you are not sure, ask!
  - Try to be sure you understand the challenge and ask for clarity as soon as you can. However, if you've missed something, you can always send a follow up email that explains the uncertainty you are having and ask for clarity
- Being too creative with your code
  - Avoid your own unique code formatting
  - Building a mobile app when you were asked to build something in the browser
  - Using an obscure new technology that no one has heard of, stick to the mainstream tools, libraries and techniques
- Copying code

  - There are many tutorials out there that may show you how to build a weather app or similar to the project you are building
  - Never submit a tutorial
  - Never submit a demo app
  - You can use a tutorial to learn things. But then you should close the tutorial and close the code examples down and then build your own version
  - If you get caught using someone else's code the interview is over
  - If you submit something above your skill level and get the job you will not last long at the job
  - If you end up using a small piece of code from Stack Overflow, make sure you can explain it

    - Better: write your own version of the code (if you can't write it, keep studying it until you can)

- Coding without preparation/planning

  - It may feel like you don't have time to plan, but planning is what will help ensure you complete the task in a sensible way that adheres to the specifications

### Summary

- Read the instructions
- Get clarifications
- Plan
- Build a simple hello world app and make sure all your configuration is set up (git/github, database, deployment etc)
- Create a README.md with clear steps on how to get your app up and running
- Make sure you build the most basic version of the app
- Polish the basic version
- Add a small write-up in the readme about the project
  - Design decisions
  - Examples
  - Potential improvements
  - [An example of a write up](https://youtu.be/DU0LAeq0Uc8?t=379)
- If you have time, try adding even more polish or a challenge recommended in the take-home assignment
- Submit it on time/early

- [The Essential Guide to Take-home Coding Challenges](https://www.freecodecamp.org/news/the-essential-guide-to-take-home-coding-challenges-a0e746220dd7/) - **CAUTION** links inside this document for `Ultimate Guide` seem to be broken/ reroute to advertisements (Spring 2022)

- [How to Pass a Take-Home Coding Test]
