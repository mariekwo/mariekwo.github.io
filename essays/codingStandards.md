---
layout: essay
type: essay
title: "Fitting a Square Peg in a Round Hole"
# All dates must be YYYY-MM-DD format!
date: 2026-02-11
published: true
labels:
  - Programming
---

<img width="200px" class="rounded float-start pe-4" src="../img/essay-img/square-peg.png">


Working in a team can be extremely frustrating. Haven't we all been there? You expect a teammate to one thing and then they do another. Or the worse case-nothing at all! Sometimes you'd rather they actually didn't do aything because what they submitted just made more work for you... am I relaying too much of my bitterness here?

A big issue when working with other people is differing standards. Not only in quality but in the way things are done. When different people write different parts of a report it can be jarring to transition between them. In coding, this transition is even more jarring.

## Good Code

Coding standards are not only important when combining the work of multiple coders, they're also important for improving readability. This is critical when other people read your code or when future you is reviewing your code. In my aforementioned experience it took longer to untangle the code contribution than it would've taken to just write it myself. I had provided a function prototype of what my code needed but the function I got back had completely different parameters. When I tried to troubleshoot the code the formatting was all over the place. It was a struggle and a lesson on the importance of code readability.

## Forced Good Code

Nowadays there are formatters like Prettier that will automatically format your code. There are also linters such as ESlint that will enforce code-quality rules meant to help with bugs. Personally I've found these tools to be very helpful and, though I haven't used them this way yet, are sure to be a great tool when working in teams.

I've recently been using ESLint with VSCode to help with TypeScript coding. There was an initial hiccup with the settings that caused my code to be formatted incorrectly but after some googling I was able to fix the issue. On the whole I quite like seeing and fixing the ESLint errors. I'm of the opinion that if you know how to fix something you can then break more complex things! Then learn to fix those and break others and so on. 

To me ESLint is a sort of middle ground between asking AI for help with code and just stumbling around on Google looking for what's wrong. And just like AI it's another tool I'm looking forward to figuring out how to use to its full potential.
