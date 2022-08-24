## React and Forms

[React Docs - Forms](https://reactjs.org/docs/forms.html)


**1.	What is a ‘Controlled Component’?**

A Controlled Component is one that takes its current value through props and notifies changes through callbacks like onChange. A parent component "controls" it by handling the callback and managing its own state and passing the new values as props to the controlled component.

**2. 	Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.**

I think, we should update the state with their responses as soon as they enter them. to keep state sync with the input’s value, So when the input is changed the status will be updated

**3. 	How do we target what the user is entering if we have an event handler on an input field?**

the displayed value will always be this.state.value, making the React state the source of truth. Since handleChange runs on every keystroke to update the React state, the displayed value will update as the user types.

____________
[The Conditional (Ternary) Operator Explained](https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff)

**1. Why would we use a ternary operator?**


**2. Rewrite the following statement using a ternary statement:**

>if(x===y){
  console.log(true);
} else {
  console.log(false);
}

Now, the ternary operator:
>condition ? value if true : value if false

> x===y ? true:false;
______________

### References


[https://www.freecodecamp.org/](https://www.freecodecamp.org/news/c-ternary-operator/)


