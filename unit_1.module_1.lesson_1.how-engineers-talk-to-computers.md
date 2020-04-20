## Introduction 

Engineers make computers do something. That something meets a particular need. Large Enterprise Engineering organizations - including Engineers, Designers, Business Analysts, and Product Owners - design whole suites of applications to meet customers' needs.

There are many ways to make a computer do something. For instance, if you are designing a website, you no longer really have to know how to talk to a computer. Content Management Systems (CMS) like Wix and Wordpress enable people without any technical background to accomplish technical things. However, even today, it is not always the case an out-of-the-box application (such as SalesForce) will completely serve a company's or a customer's needs. Enter Engineers. 

The following _Module_ **How Engineers Talk To Computers** will provide a cursory introduction to computer languages and what happens to those languages when a computer reads them. Languages are the Engineer's tool for making a computer do something. As you will learn, we can use languages to make computers do a whole lot. What language we use and how that language is used will be explored in later Lessons. This _Module_ seeks to establish a baseline of knowledge on top of which the Boot Camp will aim to build.

### Objectives

By the end of this Module, participants will be able to:

- [ ] explain why we call a programming language a language
- [ ] explain the various stages of language compilation and interpretation
- [ ] offer a few examples of "artifacts" generated as a result of writing a computer program or explain how a program is executed.

### Additional Resources

Much of what is covered below can be learned in the context of studying the JavaScript language (a language this Boot Camp will cover, extensively. 

- The [first lesson of Andrea Neagoie's Advanced JavaScript Concepts](https://www.udemy.com/course/advanced-javascript-concepts/) covers the below concepts, extensively.
- When you are more comfortable with the JavaScript ecosystem, _[Loupe](http://latentflip.com/loupe/)_ is an online tool worth examining to solidify your understanding of underlying concepts.

## Learning A New Language

Microsoft's SQL (according to the American National Standards Institute (ANSI) properly pronounced as "S-Q-L"; though most say "sequel") is based on the groundbreaking work of [Dr. E.F. "Ted" Codd](https://en.wikipedia.org/wiki/Edgar_F._Codd) (the father of relational database paradigms - about which you will learn more, later). SQL as a standard language was first implemented by IBM in the mid-1970s, with the first commercially-available implementation made available in 1979 by Relational Software Inc. (later the Oracle Corporation). Importantly for our discussion, below, [SQL is not a language - it is a standard](https://docs.oracle.com/cd/B28359_01/server.111/b28286/intro002.htm#SQLRF50928). The SQL standard resulted in many implementations (uses), many of which you will hear of in your career in technology, such as MySQL, Microsoft SQL, etc. The purpose of the SQL standard was to provide "a common language for all relational databases". Believe it or not, the first version of the SQL standard was actually called [_SEQUEL (Structured English Query Language)_](https://en.wikipedia.org/wiki/SQL). So, why all this context? 

Note the word "English" in the original SEQUEL name. Yes, many of the keywords in the SQL standard are English-based, such as SELECT, INSERT, CREATE, etc. This was entirely intentional. It was not simply that the authors of the standard were English speakers that the name of the English language made it among the first implementations. Rather, the standards authors intended for the SQL language to mimic the language with which its consumers were already very familiar. The question was asked: how closely can we mimic a natural language?

:pushpin: **Note** :pushpin:    

> Some Engineers do not refer to SQL implementations as a "language" as a SQL implementation was never meant to stand on its own - the "language" is not capable of facilitating the development of a standalone application For this reason, SQL implementations are sometimes known as sublanguages. 

You are about to learn a new language. The term language in programming may not really conform to what you may traditionally understand as a "language"; however, we use the term language as they are exactly that, languages. The languages you are about to learn have syntax, grammar, and conventions. Each component may at first look strange; but each component plays an integral part when it comes time to communicating with other people and to a computer.

When programming languages were born, computers were much slower and had much less memory. The size of a programming file (how many words) really mattered: if the size was too large, the computer couldn't process it. This impacted the way programming languages could be written - as well as other considerations for predictability of a language when the language needs to be interpreted later by a computer. As a result - while programming languages such as SQL do their best to mimic linguistic expectations - they do have to make some concessions for the sake of space. Programming languages are terse; however, when broken down into each of their constituent components, many programming languages share many of the same traits. 

So, remember: we call a programming language a "language" for a reason. As you begin down the journey of this Boot Camp, you are learning - among many things - two primary things:  (1) the hard skills needed to compete in today's market as an Enterprise-level Engineer; and (2) how to break apart the larger, sometimes seemingly-insurmountable concepts into smaller, digestible concepts that can be applied across many contexts.

## How Languages Work

The foundational language of this Boot Camp is JavaScript (eventually turning to Microsoft's [TypeScript](https://www.typescriptlang.org/)). Both of those languages behave in two very distinct ways. The focus of this **How Languages Work** section will be JavaScript. How languages work is a very deep topic and one that is addressed in many University curricula; the following overview of how will be fairly surface level and hopefully equip you with enough knowledge "to be dangerous" and to answer some more fundamental programming questions. 

For this discussion, we will be focusing on a very basic JavaScript program (to which we will return in more detail later in the Boot Camp; don't worry if you don't understand much of it, at all):

```javascript
class Hello {
    main() {
        console.log("Hello, World");
    };
}
```

### High-Level vs. Low-Level Programming Languages

There's a lot there: curly-brackets ("mustaches"); random words; something in quotation marks; oddly-placed periods. But what you are reading shouldn't look entirely foreign; there are words that look familiar - words you've probably seen in different contexts: `class`; `console`; `log`. In some very limited respects, the above "block" of code resembles the English language; or - said differently - words from the English language appear in the above block of code. If you had to guess, what would you say this code is doing?

You might be thinking something along the lines of: it looks like something - maybe the phrase "Hello, World!" - is being written (whatever that means). If so, you're absolutely right. The details of what all of it means will be explored later. But, for now, it is sufficient to know that: (1) the above code does something; and (2) it looks like it is "writing" something (whatever that means). This sense of familiarity is the most important aspect of well-written code in languages like JavaScript (and, again, is something to which we will return later in this Boot Camp) and is the primary reason we have languages like JavaScript. JavaScropt is a high-level programming language. In simple terms, JavaScript feels more natural and allows us to write something that is closer to the way we think, write, and read as humans.

"What are you talking about!" you might exclaim when hearing any programming language described as more "human". What can more human possibly mean? Let's look at the same code in a low-level programming language:

```cpp
b8          21 0a 00 00 
a3          0c 10 00 06 
b8          6f 72 6c 64 
a3          08 10 00 06 
b8          6f 2c 20 57 
a3          04 10 00 06 
b8          48 65 6c 6c 
a3          00 10 00 06 
 
b9          00 10 00 06 
ba          10 00 00 00
bb          01 00 00 00 
b8          04 00 00 00
cd          80
 
b8          01 00 00 00 
cd          80
```

Big difference, right? The above two programs do the exact same thing; however, one is - with enough training - more easily consumable to the human mind than the other. Of course, high-level languages do more things for us as programmers - but this is just enough to get you thinking about how we talk to computers and what happens in that process. Eventually everything gets boiled down to a lower-level language: a language that is more meaningful to a computer than a human. That process is known as compilation. 

## Compilation

JavaScript - the foundation of this course - is a contentious language, particularly when it comes to the question: is JavaScript a _compiled_ language or is it an _interpreted_ language? Well, the answer is "both". 

The JavaScript ecosystem is one of the most-poorly understood aspects of JavaScript languages - so much so that at [JSConf EU](https://2019.jsconf.eu/) Philip Roberts gave an entire, now-viral presentation about the JavaScript ecosystem called _[What the heck is the event loop anyway?](https://www.youtube.com/watch?v=8aGhZQkoFbQ&feature=emb_logo)_ addressing one aspect of the JavaScript ecosystem (and a highly-recommended watch for anyone participating in this Boot Camp). An understanding of these concepts including interpretation and compilation - applies to most languages. 

For your purposes, when thinking about "interpretation" vs. "compilation" it is best to understand their objective: both attempt to _take human-understandable code and convert that code into machine-understandable code_ - the difference is "what" each does and - importantly - "when". 

An interpreter: reads the file (a set of instructions) line-by-line _on the fly_ - while doing this, the interpreter translates what it encounters. So, how does this differ from a compiler? A compiler does **not** translate on the fly. It looks at the code during a compilation process (ahead of time), inspects what it sees, and "boils it down" (translates) it into different code - actually composing a _new_ program in a _new_ language (an artifact). Eventually, that new program in that new language (a lower-level language) will be interpreted when it is executed. 

"Wait a minute!" you might say. "Interpeted?" 

That's right. At some point in any code's life cycle it must be interpreted to machine-understandable code that can actually be executed by a computer as a set of instructions.

JavaScript - as mentioned earlier - is both interpreted and compiled. To understand more about how JavaScript is "both" [read about the JIT (Just-in-time) compiler](https://hacks.mozilla.org/2017/02/a-crash-course-in-just-in-time-jit-compilers/).
