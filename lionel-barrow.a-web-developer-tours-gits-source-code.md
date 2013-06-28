# A Web Developer Tours Git's Source Code

## By Lionel Barrow

### Abstract

The Ruby community has gotten pretty good at thinking about design patterns and best practices for building web applications. But many of us have little to no experience writing other types of software. That's too bad -- because many of the best ideas in web development, like the MVC pattern, can be derived from more general ideas in software engineering.

Just like how it can be hard to understand a theorem after working through only a single equation, it can be tough to understand these more general ideas when the only programs we ever think about are web apps.

In this talk, we'll look at the architecture of a non-web-app program that many Rubyists use every day: the git source control system. We'll examine the problems git is trying to solve and the constraints it faces, and we'll try to tease out how these considerations affect they way git's code is organized. We'll contrast this with the goals and constraints of web applications, and try to figure out where some of the design patterns and best practices we use are coming from.

We'll be specific, concrete, and thoughtful about the lessons we take away from this exercise -- you'll walk away with much more than a vague sense that "modularity is good" and "merge algorithms are complicated". We also might learn a thing or two about git's internal data structures.

I'll be assuming some knowledge of git, but not much.

### Notes

I've never given this talk before, but I think it'll be pretty cool. I studied git's source code extensively in class while pursuing my master's degree, and I think this exercise could be super valuable and enlightening. My main concerns would be that:

* git is written in C, which people might not be familiar with. This won't be a problem -- we can talk more about what is going on and how the code is organized than diving into pointers or whatever.
* A lot of git is organized around complicated merging algorithms, dealing with edge cases, etc. This shouldn't be a problem either. Again, we can look at organizational techniques instead of implementation details.

I've only spoken at one tech conference before: I gave a talk comparing Ruby and Go at RailsConf 2013. You can see that talk [on my website](http://lionelbarrow.com/2013/05/28/what-ruby-developers-can-learn-from-go/).

### Social

* [lionelbarrow.com](http://lionelbarrow.com.com)
* [@lionelbarrow](http://twitter.com/lionelbarrow)
* [GitHub](https://GIthub.com/lionelbarrow)
