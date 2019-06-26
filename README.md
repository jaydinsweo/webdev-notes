This is the list of topics

- [HTML](#HTML)
  - [Structure](#Structure)
- [CSS](#CSS)
  - [Flexbox](#Flexbox)
  - [Grid](#Grid)
- [Javascript](#Javascript)
  - [Functional Progamming](#Functional-Progamming)
  - [Template Strings](#Template-Strings)
  - [Algorithm](#Algorithm)
- [React](#React)
  - [Hooks](#Hooks)
    - [useState](#useState)
    - [useEffect](#useEffect)

---

# HTML

## Structure

# CSS

## Flexbox

## Grid

# Javascript

## Functional Progamming

## Template Strings

Template strings (or template literals) allows embedded expressions.
Enclosed by backslash tick ` `` ` and contain placeholders (function) by `${expression}`.

```javascript
a = 5;
b = 10;

console.log(`a + b is ${a + b}`); // a + b is 15
```

## Algorithm

Algorithm is a sequence of steps that the programm run in that particular order to achieve a particular outcomes. To solve problem, you need to break the problem down into manu chunks. For example, if the goal is to build a calculator, it would be easier to determine each arithmetic operation one by one rather than the whole.

1. Convert Celsius to Fahrenheit
   The rule to covert between these two tempetature measures is
   $$F = \frac{9}{5}C + 32 $$

<details><summary>Answer</summary>

</details>

2. Reverse a String

<details><summary>Answer</summary>
1. Turn a string into an array `array = str.split(``)`
2. 
</details>

# React

## Hooks

What is the purpose of hooks in react?

- Hooks allows to use _state_ without writing a class component.
- Hooks allows to reuse _stateful logic_ without changing component hierarchy.
  What is a state?
- [A Visual Guide to State in React](https://daveceddia.com/visual-guide-to-state-in-react/)

---

There are 4 common hooks, `useState`, `useEffect`, `useContext`, and `useRef`.

### useState

`useState` allows the function component to have the ability to use state.

```javascript
import React, { useState } from "react";

export default () => {
  const [currentState, updateState] = useState(initialState);
  const [count, setCount] = useState(0);
};
```

The `useState` has one argument, the initial state. The initial state can be number, string, booleans.
The `useState` returns a pair of values, the current state, and the function that update the state.

The state variable `count` has the value of `0`. To update the state, the `updateState` need to be call,

```javascript
<button onClick={() => setCount(count + 1)}>Click Me</button>
```

We can use {currentState} directly in the function component to display the current state.

```javascript
<p> The current count is {count} </p>
```

### useEffect

Good for read APIs, handle sync code, replace the lifecyle methods, componentdidmount, willunmount, willupdate.
scheduling after render happens - so useeffect run after return ( ). why?
don't wanna down the first render,  
useffect have to define the dependencies -

Lifecycle -
rendered first time for everything, it schedule to run useeffect later sometime
return all the markup and run the useeffect
