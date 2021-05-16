# Custom Hooks

- What does a component’s lifecycle refer to? We are born, grow, and then die. Almost everything follows this cycle in its life, and React components do as well. Components are created (mounted on the DOM), grow by updating, and then die (unmount on DOM). This is referred to as a component lifecycle.

- Why do you sometimes need to “wrap” functions in useCallback when called from within useEffect? useCallback will help in avoiding regeneration of functions when the functional component re-renders. However there isn’t much of a performance difference caused by recreation of functions.

- Why are functional components preferred over class components? Functional component are much easier to read and test because they are plain JavaScript functions without state or lifecycle-hooks. You end up with less code. They help you to use best practices.

- What is wrong with the following code?

The rules of Hooks clearly state: Don’t call Hooks inside loops, conditions, or nested functions. Instead, always use Hooks at the top level of your React function. Hooks need to be called in the same order each time the component renders.

## TERMS
-   `state hook`: A Hook is a special function that lets you “hook into” React features. For example, useState is a Hook that lets you add React state to function components.

- `effect hook`: The Effect Hook lets you perform side effects in function components:

- `reducer hook`: use sometimes to manage the state of the application. It is very similar to the useState hook, just more complex.

#### Custom hooks:
- Never call Hooks from inside a loop, condition or nested function
- Hooks should sit at the top-level of your component
- Only call Hooks from React functional components
- Never call a Hook from a regular function
- Hooks can call other Hooks 
- React Hooks with Async-Await
- We cannot use ‘async’ keyword with ‘useEffect’ callback method. It will result in race conditions.