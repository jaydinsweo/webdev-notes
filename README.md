This is the list of topics

- [HTML](#HTML)
  - [Structure](#Structure)
- [CSS](#CSS)
  - [Flexbox](#Flexbox)
  - [Grid](#Grid)
- [Javascript](#Javascript)
  - [Functional Progamming](#Functional-Progamming)
  - [Template Strings](#Template-Strings)
- [React](#React)
  - [Hooks](#Hooks)
    - [useState](#useState)


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
Enclosed by backslash tick  ` `` ` and contain placeholders (function) by `${expression}`.

```javascript
a = 5; 
b = 10;

console.log(`a + b is ${a+b}`) // a + b is 15
```

# React
## Hooks
What is the purpose of hooks in react? 
- Hooks allows to use *state* without writing a class component. 
- Hooks allows to reuse *stateful logic* without changing component hierarchy.
What is a state?
- [A Visual Guide to State in React](https://daveceddia.com/visual-guide-to-state-in-react/)
-- -- --
There are 4 common hooks, `useState`, `useEffect`, `useContext`, and `useRef`. 
### useState
 `useState` allows the function component to have the ability to use state.

```javascript
import React, { useState } from 'react';

export default () => {
    const [currentState, updateState] = useState(initialState)
    const [count, setCount] = useState(0)
}
```
The `useState` has one argument, the initial state. The initial state can be number, string, booleans. 
The `useState` returns a pair of values, the current state, and the function that update the state. 

The state variable `count` has the value of `0`. To update the state, the `updateState` need to be call, 
```javascript
<button onClick ={ () => setCount(count+1) }>
    Click Me
</button>
```

We can use {currentState} directly in the function component to display the current state. 
```javascript
<p> The current count is {count} </p>
```
