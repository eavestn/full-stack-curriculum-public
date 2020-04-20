# Unit 1, Lesson 2, Module 2: Variables And Types

## Introduction 

Variables and types is perhaps the most critical topic in any language. And - in JavaScript - there aren't any. Well, that's not actually true; but we'll learn why you can _sort of_ say that in this lesson. But, to start, let's dive into the basics. 

Programming languages - as discussed in Unit 1 Module 1 Lesson 1 _How Engineers Talk To Computers_ - are just ways for you and me to describe the world around us, like any language, whether that be Chinese, Greek, or English. And - in some sense - when we lookg a little more deeply at the way we describe things in languages, we are really only describing two things: [1] a thing; and [2] what that thing is doing: 

> Timmy is throwing the ball.

Yes, as with any language the whats, the whos, and the how-manies are more complex than those two simple things but, as you will see, you can accomplish a lot with just those two aspects of a language. This Module, _Variables And Types_ will focus specifically on the _thing_ aspect of the JavaScript language - something we will spend a lot of time on in the next three modules.

### Objectives

By the end of this Module, participants will be able to:

- [ ] clearly explain the purpose of a variable
- [ ] define a variable in JavaScript
- [ ] describe what Engineers mean when we say `type`.
- [ ] briefly speak to what JSON is (_more will be learned about JSON in later modules_).

## Properties Of A Ball

Think of a ball. What is it? Literally take a minute to pause, think, and describe a ball aloud. Chances are you will or did use terms like: diameter; circumference; size; "red", "blue", or "green"; "round"; etc. You are describing _properties_ of a ball. In most programming languages, we can do the same thing: we can _describe properties_ of a real-life object (though unless we were developing a video game or sports-based application maybe "ball" isn't the right metaphor choice). And, like in any written language, we use text to write about those properties:

```javascript
var color = "green";
var size = 4;
var units = "feet"; // <--- that's a huge ball!
```

Sure, there is some grammar and syntax above you may not recognize, but we are getting a bit closer to understanding what role variables play in languages. The simple point above is that we can use programming languages to _describe_ (in their own way) _properties_.

### purpose: storage of information

We'll get into the actual execution or "running" of a program later, but an important thing to learn early is that programs don't run forever without some help. In JavaScript, we run a file (the program) through something called a JavaScript Engine. The Engine reads in the file, looks at each line and runs each line as the Engine encounters it, then - when finished reading each line of the file - stops. Anything the file tells the Engine (instructions) to do only hangs around for as long as the Engine is running (and even this gets a bit more complex).

As the Engine is running our code, we want a place where we can share information with other parts of our code. If I say that `a ball is green`, maybe I need to make a decision about what to do with that ball, later. Variables help us accomplish just this. Variables - when read - say to the Engine, "hey, set a place for me." That place is then given the value by the of whatever we need it to be. Until the Engine is done, that variable will be around for use later.

All of this is happening in computer memory used by the code the Engine is running. 

https://dev.to/arthurbiensur/kind-of-getting-the-memory-address-of-a-javascript-object-2mnd

Can't access for security reasons.

[ parts of a variable -- create a diagram]


something to hold information - a place in memory on the computer.

Starting with _describing_ a thing -- what aspects do we have? variables first (then eventually types) --> leading into more complex types.

### Variables

#### 

##### Quick Remark 

you may see `let` vs `const` vs `var` (don't worry about that now, we'll get into that, later)

### Types
