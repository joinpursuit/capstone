# Paring on a Take Home

## Why a Pairing Activity?

Interviewers are interested in how you work with others. Do you collaborate well? Do you take feedback well? Are you adaptable and open to the style of coding at their company?

One way they can check for this is by giving a practical activity such as going over your take home challenge and then asking you to collaborate with someone to add a feature or update your code based on a code review.

When asked to pair, the goal isn't to impress the person with your coding skills silently. Rather, it is to actively collaborate and incorporate ideas, suggestions, and code from the person you are paired with. Additionally, employers are looking to see how you approach a problem as well as how you communicate about code.

## How to approach pairing

On a take home, you will typically be the person in the "driver's seat" when it comes to pairing. This means you'll be making the decisions of how to move forward on implementing a feature.

It's best to approach pairing in the same way you would approach a technical problem: identify the problem, make a plan, implement the code, and then reflect back.

### Identify the problem

First, you will want to make sure that you understand the problem you are being asked to solve or the feature you are being asked to add. For example, if you are being asked to add a signup form to a page, you will want to gain clarity around the design and any required features. Before you start coding, you should feel confident that you know what it is you're attempting to build.

### Make a plan

Before coding, it's useful to think through what exactly it is you're going to do. This could look like talking through the implementation with your pairing partner before starting, writing pseudocode to outline your potential code solution, or doing both. Making a plan _before_ you start coding will be helpful in making sure you've thought through everything. It also provides an opportunity for your partner to make suggestions or correct any misconceptions you may have.

### Implement your code

Now is the time for you to actually write some code. During this phase, you will likely be doing most of the typing. However, as best as you can, talk through what you're doing so that your partner can follow along.

One of the benefits of doing a take home challenge is that you're often not required to have memorized every bit of syntax. If you get stuck or can't remember how to do something, feel free to ask your partner. In a real pairing situation, your partner should be willing to look up syntax and point out any small mistakes that could cause problems.

### Reflect back

Once the problem is solved or the feature has been implemented, it's time to reflect back on what you just solved. Depending on the type of challenge, you may be asked to just reflect on what could be improved or you may be tasked with refactoring your code. Either way, this is an opportunity to highlight your skill at improving code to be more readable as opposed to just getting it to work.

## Ways to improve your code

Coding design has to do with following some good principles like writing clean and clear code, "YAGNI", "DRY" and "KISS."

Let's review these principles, so that as you talk through your code you can help identify some of the design choices you are making.

### Clean Code

Writing clean code usually refers to your ability to do the following:

- Name variables and functions in a way that express intent and improves clarity
- Write and structure your code so that it requires as few comments as possible to understand

For example, take a look at the following function which adds two numbers togethers.

```js
// This function adds two numbers together and returns the value
const x = (y, z) => z + y;
```

The above function is _concise_ but lacks clarity. The function name (i.e. `x`) tells us nothing about what the function is. The comment is needed because variables `y` and `z` don't give any indication as to the data type that is expected. And, the order of parameters and how those parameters are used are flipped.

Contrast the above function with the following:

```js
const addTwoNums = (num1, num2) => num1 + num2;
```

This function is much better. The name of the function describes its purpose and the parameters names give some indication as to how it should be used. This code is still concise but is much more clear.

For longer snippets of code, it's possible that the code will be difficult to read not because of poorly named variables but because of the unclear intentions behind the code. For example, take a look at the following code below which will increase a value stored in an object by a certain percentage.

```js
function increasePrice (product = {}, percentageIncrease = 0) {
  if (product.priceInCents && product.priceInCents > 0) {
    if (percentageIncrease >= 1) {
      throw "percentageIncrease must be between 0 and 1.";
    }
    if (percentageIncrease < 0) {
      throw "percentageIncrease must be between 0 and 1.";
    }
    
    product.priceInCents *= (1 + percentageIncrease);
  } else {
    throw "priceInCents is missing or formatted incorrectly.";
  }
}
```

This function performs a lot of error handling to make sure the values entered are properly set. While necessary, these checks obscur the true purpose of the function which is simply to increase the `priceInCents` key-value pair.

There are a few approaches you could take to improve the readability of this code. One might be to use guard clauses at the beginning of the function. A guard clause stops the execution of some code early on so that the rest of the function doesn't run. In addition to at times being more performant, it also has the added benefit of improving deeply nested code.

```js
function increasePrice (product = {}, percentageIncrease = 0) {
  if (!product.priceInCents || product.priceInCents < 0) {
    throw "priceInCents is missing or formatted incorrectly.";
  }
  if (percentageIncrease >= 1) {
    throw "percentageIncrease must be between 0 and 1.";
  }
  if (percentageIncrease < 0) {
    throw "percentageIncrease must be between 0 and 1.";
  }
    
  product.priceInCents *= (1 + percentageIncrease);
}
```

These changes improve the overall clarity of the function by moving all of the error checking to the front of the function. Even more can be improved by removing some duplicate code.

```js
function increasePrice (product = {}, percentageIncrease = 0) {
  if (!product.priceInCents || product.priceInCents < 0) {
    throw "priceInCents is missing or formatted incorrectly.";
  }
  if (percentageIncrease >= 1 || percentageIncrease < 0) {
    throw "percentageIncrease must be between 0 and 1.";
  }
    
  product.priceInCents *= (1 + percentageIncrease);
}
```

The code above is certainly an improvement from the original code. However, you could reorganize your code even further by using helper functions.

```js
const validateProductPrice = (price) => {
  if (!price || price < 0) {
    throw "priceInCents is missing or formatted incorrectly.";
  }
}

const validatePercentage = (percentage) => {
  if (percentage >= 1 || percentage < 0) {
    throw "percentageIncrease must be between 0 and 1.";
  }
}

function increasePrice (product = {}, percentageIncrease = 0) {
  validateProductPrice(product.priceInCents);
  validatePercentage(percentageIncrease);
  product.priceInCents *= (1 + percentageIncrease);
}
```

This code uses helper functions to encapsulate the various error checking. Those helper functions are then used inside of the original function.

In this specific situation, building helper functions may not be necessary. However, if those validation functions could be used again, this could be a great way to clean up the code.

For more on cleaning up `if` statements, you may want to view the following video:

- [Cleaner IF statements// Clean Code](https://www.youtube.com/watch?v=2QWMrEHoMFA)

### Acronyms

There are a few key acronyms that are helpful to keep in mind as you refactor or improve your code.

#### YAGNI

This acronym stands for "[You aren't gonna need it](https://en.wikipedia.org/wiki/You_aren%27t_gonna_need_it)."

This saying is trying to convey that it is important to stay focused on the required features as opposed to setting up your code for features that may exist in the future.

#### DRY

This acronym stands for "[Don't Repeat yourself](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself)."

The intention behind this saying is that you should look for code that is repeated and, wherever possible, remove it.

#### Kiss

This acronym stands for "[Keep it Simple](https://en.wikipedia.org/wiki/KISS_principle)."

The intention behind this saying is to prioritize simplicity over complexity when solving a problem. Being able to write things in a simple and clear way demonstrates more skill and depth of knowledge than writing a convoluted or confusing answer. It also makes the code more readable and maintainable.

## Resources

- [How to Pair Program](https://www.wikihow.com/Pair-Program)
- [7 Tips for Navigating a Pair Programming Session During a Job Interview](https://www.techrepublic.com/article/7-tips-for-navigating-a-pair-programming-session-during-a-job-interview/)
