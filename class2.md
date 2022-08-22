## React lifecycle
______

#####  Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?

according the diagram the **_render_** occur first then **react updates DOM** and finally **componentDidMount**

##### What is the very first thing to happen in the lifecycle of React?
constructor() : The constructor for a React component is called before it is mounted.

constructor() -> static getDerivedStateFromProps() -> render() -> componentDidMount()


##### Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates

_Mounting phases:_
constructor -> render -> React Updates -> componentDidMount

_Unmounting phases:_
componentWillUnmount


##### What does componentDidMount do?
If you need to load anything using a network request or initialize the DOM, it should use _componentDidMount()_. This method is a good place to set up any subscriptions.

## React State Vs Props
______

##### What types of things can you pass in the props?
Props allow you to pass data from one component to other components as an argument.

##### What is the big difference between props and state?
state is internal while props are external & state is  controlled by the component itself while props are  controlled by whatever renders the component

##### When do we re-render our application?

When the state changes in the parent component 

##### What are some examples of things that we could store in state?

A count, like (time). Because we need to change it constantly

##References
_______

[https://www.javatpoint.com/](https://www.javatpoint.com/react-state-vs-props)