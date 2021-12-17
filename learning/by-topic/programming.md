---
title: How to Learn Programming
description: Some advice about learning programming with spaced repetition.
published: true
date: 2021-12-17T17:38:52.689Z
tags: programming, computer-science
editor: markdown
dateCreated: 2021-12-17T17:38:52.689Z
---

# How to Learn Programming with SRS

These are some notes on learning to program with SRS based on my own experience as well as observing others teach themselves programming with SRS. Feel free to edit! Get in touch with me [on Twitter](https://twitter.com/experilearning) or on Discord (Jamesb#7557) if you want to discuss!

## Most important points:

- 80-90% of your time should be spent working on your own projects.
- 10-20% of your time should be spent doing IR / flashcards / watching lectures or tutorials.

You cannot learn programming through flashcards and reading alone. Programming is a applied discipline where much of your expertise is gained tacitly through practice rather than through reading books. That's not to say that flashcards and incremental reading are not worth investing in - they might double or triple your programming knowledge in the long run but only if you are actively working on non-trivial projects that are interesting to you at the same time.

#### See Also:

Here are some additional resources about SRS and programming you might find interesting:

- Article: [SuperMemo as a Tool for a Programmer](https://supermemo.guru/wiki/SuperMemo_as_a_tool_for_a_programmer) by Piotr Wozniak
- Reddit: Reddit user SigmaX's [comments on Reddit](https://www.reddit.com/user/SigmaX/) where he shares examples of programming cards.
- Blog: Reddit user SigmaX's [blog](https://ericsiggyscott.medium.com). He has a couple of articles on using SRS to learn programming and machine learning.
- Blog: [A guide about using Anki to learn programming which the author calls the "Janki Method"](https://www.jackkinsella.ie/articles/janki-method).
- Blog: [Another guide about using Anki to learn programming](https://sive.rs/srs)

## Projects

- The first project I would recommend is writing a blog - not only will you learn programming, but you will also have a place to write about what you learned and show off your portfolio. So just by having a blog you already have multiple couple of projects you can show to a potential employer.,
- The big advantage of free learning is that you are able to choose what you want to work on, so choose things that you are personally interested in. For example, if you are interested in crypto, why not make a simple crypto investment tracker dashboard.
- I don't recommend copying tutorials line by line - a strategy I have personally found more useful is taking a tutorial that is related to what I want to do, and then change it in some way - eg. by  using a different programming style, a different set of technologies, or taking a different angle. So if your goal is to create a crypto dashboard, you could look up tutorials to create a normal stock tracker and adapt it to track crypto instead.
- Someone messaged me recently with an idea called "structured imitation" where you watch a tutorial, but pause before the teacher shows you how to build something and try to actually predict what they are gonna do and build it yourself before watching the teacher do it. 


## Important Concepts

These are some examples of some of the most important "language invariant" concepts, ie. those that are shared between most programming languages. You want to prioritize fundamental, generally applicable knowledge because it will help you reason from first principles and solve problems you haven't seen before. Some of the ones I listed (eg. concurrency and mutable vs immutable data) can also be a source of very painful bugs if you don't understand them deeply.

- Mutable and immutable data, call by value, call by reference, pointers
- Basic data structures: list, dictionary, set
- Classes, interfaces, inheritance (for OOP languages)
- Lambda functions, closures
- Async/Await and concurrency
- Higher order functions including the classic functional programming higher order functions - at least map, filter, reduce

## Incremental Reading for Programming

The goal is to create an immersion environment of high quality info which will incrementally expose you to more advanced concepts.

- Explore rabbit holes, import interesting stuff into SM, import and postpone stuff that looks important but you can't understand yet.
- Use Wikipedia and books for the theoretical side. It's densely connected, shows the links between CS, math, logic and the practical side of coding.
- High quality blogs for the street knowledge - stuff you can't find in documentation, explanations of the fundamentals, explanations of useful design patterns to improve your code etc.

Here's an example of stuff you could incrementally read to learn C#:

### Passive Learning (IR/IV) for C#

- High quality books: C# in a nutshell, C# in depth
- Blog posts by: Eric Lippert, Jon Skeet, Stephen Cleary, Stephen Toub, Marc Gravel, [Alexey Golub](https://tyrrrz.me/)
- Import interesting threads answered by the C# language designers or C# experts. Eg. You can do queries on StackOverflow to find posts that are answered by multiple knowledgeable people
    - [Questions answered by both Jon Skeet and Eric Lippert](https://data.stackexchange.com/stackoverflow/query/166045/questions-that-have-been-answered-by-both-jon-skeet-and-eric-lippert)
- [Some twitters are also very relevant](https://twitter.com/EgorBo/status/1305986533154000904). Once you follow one you get suggestions for more.
