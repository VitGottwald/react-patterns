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

React is all about components. And components are all about reuse. One of the methods to reduce repetition and achieve greater reuse is a _separation of concerns_. Over time various repeating patterns have been identified and given a name.

## Container/Markup components

The first pattern we come across that separates the concerns of
1. **fetching data**
2. **rendering user interface**

Fetching data is the responsibility of *Container* components and rendering user interface is the responsibility of *Markup* components. It is nicely described in [this article](https://link.medium.com/fwP1izSYGT).

## Container/Presentational components

This is a generalization of the previous pattern, described by Dan Abramov in [this article](https://link.medium.com/PHW833Q6GT).

## Functional/Class Components

Components can be written either as regular functions or as Classes. Functions are thhe most staightforward way to create a component. But they have some limitations. This has to do with performing side effects

## Stateless/Stateful Components

## Pure/Not Pure components

*Pure component* is a component that does not depend on any externally changing data, except the propeties it receives, and its internal state (managed by setState calls). This definition requires a little bit more elaboration.

Functional component (NOT using hooks) may or may not be pure. This depends on whether it reads data from a source, that may change over time, other that its props (e.g. window, or a another variable declared outside its function body). 

Because react is calling components during render we do not have control when a it is called. Hence creating a functional component that is not pure does not seem to make sense because we could be getting random results at various render calls and our UI would become unpredictable. There is one exeption to this. When we call functions that react expects us to call during render. Such calls can be managed by react and an example of this is react hooks.

Class component, with, or without an internal state (managed by setState) may or may not be pure as well. Again, it depends on whether the component reads data from a source that may change over time, other that its props.

A pure component may only read data from its props, its internal state, and external data that does not change over time.


