# Class 02: State and Props

## React Lifecycle

### Based off the diagram, what happens first, the 'render' or the 'componentDidMount'?

Based on the diagram provided entitled "React Lifecycle Events", the `render` happens before the `componentDidMount`.

### What is the very first thing to happen in the lifecycle of React?

The very first thing to happen in the lifecycle of React is the **Mounting** phase; specifically the mounting of the **constructor**.

### Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates

1. constructor
2. React Updates
3. render
4. componentDidMount
5. componentWillUnmount

### What does componentDidMount do?

The `componentDidMount` is called immediately after the component is mounted and is used to load data from network requests.

## React State vs Props

### What types of things can you pass in the props?

Props are similar to parameters in a function; therefore, you can pass the same things to it as you would a function.

### What is the big difference between props and state?

State is handled in the component and updated inside of the component.
Props are handled outside of the component, and updated outside of the component.

### When do we re-render our application?

A re-render occurs when the state or props of a component change.

### What are some examples of things that we could store in state?

* User input
* Toggles
* Counters

## Things I want to know more about

Nothing at the moment
