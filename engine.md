# Creation of a RegEx Engine

In this part we build several RegEx engines from scratch. There are multiple ways of doing this and this implementation is far from production ready. See this part as a possibility to learn, how a RegEx engine might work in principal. If you need a RegEx engine in production code, use what is available in your programming language and do not create your own engine.

## What is the RegEx engine?
If we use a method from the RegEx module like `re.match(r"^\d\d:\d\d", "12:55")` this will be processed by a RegEx engine which 'understands' all the specific meta characters, quantifiers etc. We call these things **units** during the course. The unterstanding of these units by the RegEx engine typically consists of two steps: first the transformation of the RegEx into a machine friendly syntax and a simulation run of the input text with this created machine as a second step. 

## Multiple types of RegEx engines
There are multiple types of RegEx engines: one type is a **DFA**, another type is a **NFA** machine or you can implement RegEx using a recursive approach. 

Every engine differs in the way how simple they are to built, how fast they can deliver a valid result and how powerful they are. A RegEx engine is more powerful if it supports more special characters or features like lookahead and lookbegind.

We start by implementing a **DFA** regex machine. 

[Overview](./overview.md) | [Next (DFA)](./engine/dfa.md)

