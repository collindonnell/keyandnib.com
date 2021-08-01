---
layout: post
title: An iOS Developer Learns Ruby (Part 1)
---

I've been coding Objective-C professionally for thirteen years and Swift for five-and-a-half. I've also dabbled in Python for almost as long as I've done Objective-C, although never professionally. My experience with Python is writing lots of little scripts and quite a bit of dabbling with Django. More recently, however, I've been learning Ruby, and honestly, I like it.

I've wanted to take the time to get good with a web framework. I also thought of really mastering a language that could replace shell for most of my scripting needs. Another reason is that my friend [Samuel](https://twitter.com/samuelgoodwin) kept telling me how great Rails is, and I've wanted to learn web development for a while now.

## Simplicity

So why, after trying both, have I decided to go deep on Ruby and not Python? The biggest reason is that it just _spoke_ to me more. For how synonymous with simplicity Python is, that hasn't been my experience. 

Ruby is a lot more dynamic, but as someone who's done a lot of Objective-C, the things people talk about being **magic** in something like Rails make sense to me. Ruby makes it easy to do things like add methods at runtime, and so if you get how that kind of stuff works, the fact Rails can have **article\_params** available because you called you're working with **Article** objects in **ArticleController** makes total sense. If you understand a few rules, there's not much to remember in Ruby, from what I can tell.

In Ruby, everything is an object, and you use the dot operator for message passing. Variables are private by default; if you need to make them accessible, you can add **attr\_reader**, **attr\_writer**, or **attr\_accessor** (read and write). If you need something more specific, you can write custom accessors.  

In Python, instance variables are public, but there's also **property()**, which has a wrapper called **@property**, and you can also write accessors. I understand the difference, but I'm also never clear on when to do one thing or the other. If you want "private" instance variables, that means putting underscores in front of the name — but that's just a convention — it doesn't do anything.

Another weirdness in Python that adds to its cognitive load is that it's not _entirely_ object-oriented. Sometimes you use a method, but other times — **len()** to get the length of an array or string — they're global functions. In Ruby, length is always a method call.

I think Python gets called simple more because, if you've never seen either language, the syntax appears more understandable. Ruby uses weird symbols that don't make sense unless you take the time to learn what they do. The thing is this, though: I don't care what a language looks like to people who don't know it — I care how productive and enjoyable it is to use for people who **do**.

## Shell Scripting

Ruby rules for shell scripting. I don't have to import anything, and I can do useful things. Regular expressions are also built-in, and the syntax is simple. I never found Python good for one-liners on the command line; Ruby is excellent for that. For quick and dirty scripts, the ability to do things like this is amazing:

`command.match(/regex/)`

## Conclusion

The thing about languages is that they're all great, and they all suck. I probably haven't gotten far enough into Ruby to figure out what sucks about it. So far, though? It feels comfortable and fun. I think that's the best you can hope for.
