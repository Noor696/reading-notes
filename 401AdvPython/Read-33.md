## Context API

[What is Global State]()

* In React, originally, the state is held and modified within the same React component. 

* most applications, different components may need to access and update the same state.

* This is achieved by introducing the global states in your app.

*  The main purpose of **the global state** is to share a state among multiple components. 

**There are three ways this communication can happen:**
  
  - With a child component
  - With a parent component
  - With a sibling component

**State traveling down**

* State traveling down through the hierarchy is best managed using the mutable state at the highest level to determine immutable properties that define the lower-level components.

* when these properties are updated, the lower-level component is updated rather than fully recreated.

**State traveling up**

* You need to pass down a callback function for a higher-level component to know the state.

* In the following version, we add a global state to count the total number of button presses and update this state with a callback function called pushed, which is called whenever a button is pushed.

**State traveling sideways**

* Various sub-components need to communicate updates between them. This can be achieved by passing state, using callback, up to a common parent component, and then passing it back down.

--------------------

[Context API in React]()

* Context provides a way to pass data through the component tree without having to pass props down manually at every level.

* Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language.

--------------------

[Context API vs Redux JS]()

* Context API is a built-in React tool that does not influence the final bundle size, and is integrated by design.

* To use the Context API, you have to:

Create the Context -> Create a Provider for the Context -> Consume the data in the Context

* Redux is an Open Source Library which provides a central store, and actions to modify the store. we are comparing it to Context API, so we will stick to React-based Applications.

* To use Redux you need to:

Create a Reducer -> Configure the Store -> Make the Store available for data consumption -> Use State or Dispatch Actions


## Comparing Redux & Context API

| Context API  | Redux |
| ------------- | ------------- |
| Built-in tool  | Additional installation Required  |
| Requires minimal Setup  | Requires extensive setup  |
| designed for static data  | Works with both static and dynamic data  |
| Adding new contexts requires creation from scratch  | Easily extendible due to the ease of adding new data/actions after the initial setup  |
| Debugging can be hard  | Incredibly powerful Redux Dev Tools to ease debugging  |
| UI logic and State Management Logic are in the same component  | Better code organization with separate UI logic and State Management Logic  |