# Hooks API
- Why do we not need more .html pages in a multi-page React app?
because of react-router-dom Many modern websites are actually made up of a single page, they just look like multiple pages because they contain components which render like separate pages.
- If we wanted a component to show up on every page, where would we put it and why?

Inside the `<BrowserRouter />`, outside a `<Route />`,this will allow it to render on all pages regardless of a specified route.

- What does props.children contain?
Props.children is a special prop, automatically passed to every component that can be used to render the content included between the opening and closing tags when invoking a component

### TERM
`Composition`: react Composition is a development pattern based on React's original component model where we build components from other components using explicit defined props or the implicit children prop.

`Children / Child Components:` children is a special property of React components which contains any child elements defined within the component

`Hash Routing`: Hash value will be handled by react router. It is used to support legacy browsers which usually doesn't support HTML pushState API It doesn't need any configuration in server to handle routes This route isn't recommended by the team who created react router package

`Link Routing`: Provides declarative, accessible navigation around the application.

## HOOKS
Hooks are functions that let you “hook into” React state and lifecycle features from function components. Hooks don't work inside classes — they let you use React without classes. ... You can also create your own Hooks to reuse stateful behavior between different components.

- Hooks are JavaScript functions, but they impose two additional rules:

 - Only call Hooks at the top level. Don’t call Hooks inside loops, conditions, or nested functions.
 - Only call Hooks from React function components. Don’t call Hooks from regular JavaScript functions.