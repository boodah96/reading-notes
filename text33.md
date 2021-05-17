## Context API

- Describe use cases for useMemo() and useReducer() 
useReducer(): when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. It is best used when you are dealing with a complex object where individual properties need to be operated on
 useMemo(): when the data doesn’t change between renders.

- Why do custom hooks need the use prefix?
Its name should always start with use so that you can tell at a glance that the rules of Hooks apply to it.


- What do custom hooks usually do?
Custom hooks allow us to have cleaner functional components, remove logic from the UI layer, and prevent code duplication by bringing common use cases to reusable hooks.


- Using any list of custom hooks, research and name one that you think will be useful in your applications 
useToggle: change a value between true and false.used for show and hide modal, show more/show less text, open/close side menu.

- Describe how a hook that fetches API data might work 
use the useEffect and useState Hooks to fetch and display information in a sample application, using JSON server (Links to an external site.) as a local API for testing purposes. You’ll load information when a component first mounts and save customer inputs with an API

## TERM
`reducer`: is a function that determines changes to an application’s state. It uses the action it receives to determine this change.

## React Context

- Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language. For example, in the code below we manually thread through a “theme” prop in order to style the Button component: class App extends React.
- Creates a Context object. When React renders a component that subscribes to this Context object it will read the current context value from the closest matching Provider above it in the tree.

- The defaultValue argument is only used when a component does not have a matching Provider above it in the tree. This can be helpful for testing components in isolation without wrapping them. Note: passing undefined as a Provider value does not cause consuming components to use defaultValue.