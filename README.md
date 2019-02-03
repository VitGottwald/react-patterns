# The Small React Patterns Overview

(React)[https://reactjs.org/] is a javascript library for building user interfaces. It was created by Facebook to solve a seemingly simple task - to make sure your web page shows what you want it to be showing. In other words, to make sure your user interface stays in sync with your data. 

This is my personal list of original sources to use when asked by people new to react where to go to learn about a particualr pattern.

The first video I saw about react was (Hacker Way: Rethinking Web App Development at Facebook)[https://youtu.be/nYkdrAPrdcw]. If you are new to react I would highly recommend you to watch the part presented by Pete Hunt, starting at (24:18)[https://youtu.be/nYkdrAPrdcw?t=1458].

# Component patterns

React is all about components. And components are all about reuse. One of the methods to reduce repetition and achieve a greater reuse is a _separation of concerns_. Over time various people have identified repeating patterns and given them a name.

## Container/Markup components

The first pattern we come across that separates the concerns of
1. **fetching data** - Container
2. **rendering user interface** - Markup
originally described in a (medium article)[https://link.medium.com/fwP1izSYGT]

