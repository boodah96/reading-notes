# Routing
1- Do child components have direct access to props/state from the parent?
 not direct access but by pass its state as a props to the child.


2- When a component “wraps” another component, how does the child component’s output get rendered?

<Main>
  <Content />
</Main>
Gets rendered when there is an update to state.
3- Can a component, such as <Content />, which is a child also be used as a standalone component elsewhere in the application?
yes
4- What trick can a parent use to share all props with it’s children
children Using spread operator,
The parent can pass them directly to all children or pass a function to them to share all the states and props.
.


## Term
`props.children`: children elements directly into their output
`composition`: another word for writing — the act of writing or the piece of writing that results. It also refers to what something is made of. The word composition comes from the Latin componere, meaning "put together" and its meaning remains close to this.

## Router :

- React Router is a standard library for routing in React. It enables the navigation among views of various components in a React Application, allows changing the browser URL, and keeps the UI in sync with the URL.

- When starting a new project, you need to determine which type of router to use. For browser based projects, there are and components. The should be used when you have a server that will handle dynamic requests (knows how to respond to any possible URI), while the should be used for static websites (where the server can only respond to requests for files that it knows about).