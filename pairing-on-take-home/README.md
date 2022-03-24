# Paring on a Take Home

## Why a Pairing Activity?

Interviewers are interested in how you work with others. Do you collaborate well? Do you take feedback well? Are you adaptable/open to the style of coding at their company?

One way they can check for this is by giving a practical activity such as going over your take home challenge and then asking you to collaborate with someone to add a feature or update your code based on a code review.

When asked to pair, the goal isn't to impress the person with your coding skills silently, rather, it is to actively collaborate and incorporate ideas/suggestions/code from the person you are paired with.

## General Coding Design Abilities

Coding design has to do with following some good principles like, clean code, YAGNI, DRY and KISS

Let's review these principles, so that as you talk through your code you can help identify some of the design choices you are making

### Clean Code

Clean code usually refers to

- Good naming of variables and functions
- Avoiding writing unnecessary comments to clarify code that could have been written more clearly

```js
// This function adds two numbers together and returns the value
const x = (y, z) => z + y;
```

```js
const addTwoNums = (num1, num2) => {
  return num1 + num2;
};
```

- Write readable code

While the following code is short, how long does it take to understand what it is doing?

```js
someVal ? (anotheVal ? 0 : someVal && !!inputQ) : 1;
```

This code is still a bit convoluted/unclear and could be written in a more simple and clearer way. But it's easier to understand than the one line code

```js
if (someVal) {
  if (anotherVal) {
    return 0;
  } else {
    return someVal && inputQ === false;
  }
} else {
  return 1;
}
```

[Here is a video example: Cleaner IF statements// Clean Code](https://www.youtube.com/watch?v=2QWMrEHoMFA)

- Keeping the code as simple as possible

- Keep your project well-organized. Follow conventions for files, file names, folder structure and folder names. If there is a lot of variability within the tech stack, be consistent within your project

### YAGNI

[You aren't gonna need it](https://en.wikipedia.org/wiki/You_aren%27t_gonna_need_it) - stay focused on the required features. Don't try to set up your code to add eventual features that are not planned. Don't try to add extra features that are not required. Keep the code simple

### DRY

[Don't Repeat yourself](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself)

If you find a solution for what you are working on is to write similar code over and over again, take a moment to see if you can convert it into a function and/or a loop

### Kiss

[Keep it Simple](https://en.wikipedia.org/wiki/KISS_principle)

Being able to write things in a simple and clear way demonstrates more skill and depth of knowledge than writing a long convoluted or confusing answer. It also makes the code more readable and maintainable.

## Getting Started

Coding should never be the first thing you do.

Always take some time to clarify the prompt, clarify what you are doing, make sure you understand how you will be working together and anything else needed to form a productive collaboration.

## Continue Planning

Think about breaking the problem down into multiple steps and then make a plan for the order to tackle the steps. Be sure to communicate this with your partner. E.g. "First, I am going to build the route, then I will build the database query"

## Start Coding

Be sure to engage your partner. If you start writing a `for` loop, but your partner recommends a `for in` loop, talk through it and try to incorporate their idea, if you are getting stuck, talk it through.

Be mindful of your variable names, code organization and all the other best coding practices you've been learning. It's ok to slow down and do things right.

## Resources

- [How to Pair Program](https://www.wikihow.com/Pair-Program)
- [7 Tips for Navigating a Pair Programming Session During a Job Interview](https://www.techrepublic.com/article/7-tips-for-navigating-a-pair-programming-session-during-a-job-interview/)
