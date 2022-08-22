# Introduction to React and Components

#### Component-Based Architecture

##### 1.	What is a “component”?
A component is a software object, intended to interact with other components, each component perform functionality or a set of functionalities, All components contribute to the creation of the user interface.
##### 2.	What are the characteristics of a component?
Reusable; The component can be design and use in other applications, and may be for a specific application.
Replaceable; Replacing a component with another similar component.
Not context specific; Components are designed to operate in different environments and contexts.
Extensible; can be extended from existing components to provide new behavior
Encapsulated; it allows its functionality to be used without exposing its internal processes, variables or state.
Independent; Components are designed to have minimal dependencies on other components.

##### 3.	What are the advantages of using component-based architecture?
**Ease of deployment** − As new compatible versions become available, it is easier to replace existing versions with no impact on the other components or the system as a whole.
**Reduced cost** − The use of third-party components allows you to spread the cost of development and maintenance.
**Ease of development** − Components implement well-known interfaces to provide defined functionality, allowing development without impacting other parts of the system.
**Reusable** − The use of reusable components means that they can be used to spread the development and maintenance cost across several applications or systems.
**Modification of technical complexity** − A component modifies the complexity through the use of a component container and its services.
**Reliability** − The overall system reliability increases since the reliability of each individual component enhances the reliability of the whole system via reuse.
**System maintenance and evolution** − Easy to change and update the implementation without affecting the rest of the system.
**Independent** − Independency and flexible connectivity of components. Independent development of components by different group in parallel. Productivity for the software development and future software development.

#### What is Props and How to Use it in React
##### 1.	What is “props” short for?
A feature that is used to help components send data to each other, and the data is passed in a unidirectional route.
##### 2.	How are props used in React?
Define the attribute and its value (data) -> then pass it to the child component(s) using Props -> render the props data
##### 3.	What is the flow of props?
uni-directional flow. (one way from parent to child)
