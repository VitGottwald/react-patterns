# The Small React Patterns Overview

[React](https://reactjs.org/) is a javascript library for building user interfaces. 

This is my personal list of original sources to use when asked by people new to react where to go to learn about a particular pattern.

React was created by Facebook to solve a seemingly simple task - to make sure your web page shows what you want it to be showing. In other words, to make sure your user interface stays in sync with your data. And the method how to do it is best described by the following quote

> We should do (as wise programmers aware of our limitations) our utmost to shorten the conceptual gap 
> between the static program and the dynamic process, to make the correspondence between 
> the program (spread out in text space) and the process (spread out in time) as trivial as possible.
> 
> [Edsger W. Dijkstra](https://en.wikiquote.org/wiki/Edsger_W._Dijkstra)



The first video I saw about react was [Hacker Way: Rethinking Web App Development at Facebook](https://youtu.be/nYkdrAPrdcw). If you are new to react I would highly recommend you to watch the part presented by Pete Hunt, starting at [24:18](https://youtu.be/nYkdrAPrdcw?t=1458).

# Component Patterns

React is all about components. And components are all about reuse. One of the methods to reduce repetition and achieve a greater reuse is a _separation of concerns_. Over time various repeating patterns have been identified and given a name.

## Container/Markup components

The first pattern we come across that separates the concerns of
1. **fetching data**
2. **rendering user interface** - performed by *Markup* components

Fetching data is the responsibility of *Container* components and rendering user interface is the responsibility of *Markup* components.

this is nicely described in [this medium article](https://link.medium.com/fwP1izSYGT).

