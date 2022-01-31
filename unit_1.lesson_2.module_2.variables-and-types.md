# Unit 1, Lesson 2, Module 2: Variables And Types

## Introduction 

Variables and types is perhaps the most critical topic in any language. In JavaScript, despite types being the most critical topic, there aren't any. 

Well, that's not actually true; but we'll learn why you can _sort of_ say that JavaScript doesn't have types in this lesson. To start, let's dive into the basics. 

Programming languages, like any other language, whether that be Chinese, Greek, or English are just ways for you and me to describe the world around us. In some sense, when we look a little deeper at the way we describe things in languages, we are really only describing two things: [1] a thing (an object); and [2] what that thing is doing (an action): 

> Timmy is throwing the ball.

Yes, as with any language the whats, the whos, and the how-manies are more complex than those two simple things but, as you will see, you can accomplish a lot with just those two aspects of a language. 

This Module, _Variables And Types_ will focus specifically on the _thing_ aspect of the JavaScript language - something we will spend a lot of time on in the next three modules.

### Objectives

By the end of this Module, participants will be able to:

- [ ] clearly explain the purpose of a variable
- [ ] define a variable in JavaScript
- [ ] describe what Engineers mean when we say `type`.
- [ ] briefly speak to what JSON is (_more will be learned about JSON in later modules_).

## Properties Of A Ball

Think of a ball. What is it? Literally take a minute to pause, think, and describe a ball aloud. Chances are you will or did use terms like: diameter; circumference; size; "red", "blue", or "green"; "round"; etc. You are describing _properties_ of a ball. In most programming languages, we can do the same thing: we can describe _properties_ of a real-life object (though unless we were developing a video game or sports-based application maybe "ball" isn't the right metaphor choice). 

As in any written language, we use text to write about those properties:

```javascript
var color = "green";
var size = 10;
var units = "feet"; // <--- that's a huge ball!
```

You may not recognize some grammar and syntax above, but we are getting a bit closer to understanding what role variables play in languages. The simple point above is that we can use programming languages to _describe properties_ of a thing, such as a ball.

### Variable Purpose: What Is A Variable

We'll cover actually executing or "running" a program later. 

An important thing to know early is that programs don't always run forever. In JavaScript, for instance, we execute a file (the program) using something called a _JavaScript Engine_. The Engine [1] reads in a file, [2] looks at each line and runs each line as the Engine encounters it, then - when finished reading each line of the file - [3] stops. Anything the code file (instructions) tells the Engine to do only hangs around for as long as the Engine is running (and even this gets a bit more complex).

As the Engine is running our code - executing each line, following it, then discarding it - we want a place where we can share information with other, future parts of our code. If we say `a ball is green`, we may need to make a later decision about what to do with that ball, maybe even based on its color. Variables help us accomplish just this. Variables - when read by the Engine - say, "hey, set a place in memory for me." That place is then given the value of whatever we need it to be. Until the Engine is done, that variable will be around for use later.

All of this is happening in computer memory used by the code the Engine is running. In some languages, if you attempt to "read" a variable while the program is running, you will actually see the variable's address (the place where the variable lives) in memory. It'll even look a little like something only a computer could understand: `#<6C1457DBD4>` . For security reasons (protecting our code from malicious users), [JavaScript doesn't enable retrieving these addresses](https://dev.to/arthurbiensur/kind-of-getting-the-memory-address-of-a-javascript-object-2mnd).

### Variables: How To Read And Write Them

Every language has a syntax - a structure - we follow. For English learners, "syntax" should evoke horrid memories of red and blue crayons underlining the parts of a sentence. Welp. JavaScript is no exception. JavaScript has expectations about _how_ it is written. This expectation is enforced by the Engine, mentioned earlier. The syntax ensures the Engine can understand what it is that we are trying to communicate. 

We leared a moment ago that a variable intends to describe the property of something. We also saw a very quick and sneaky example of JavaScript variable syntax:

```js
var color = "green";
```

There are five pieces to the above JavaScript [statement](https://www.teamten.com/lawrence/programming/intro/intro2.html). 

[ parts of a variable -- create a diagram]

something to hold information - a place in memory on the computer.

Starting with _describing_ a thing -- what aspects do we have? variables first (then eventually types) --> leading into more complex types.


#### 

##### Quick Remark 

you may see `let` vs `const` vs `var` (don't worry about that now, we'll get into that, later)

### Types
