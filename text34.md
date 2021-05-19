## `<Login /> and <Auth />`:
- Why is the Context API useful?
  data shares global between all components of the tree.
- Can a component outside of a provider get its context?
React context is available only when the UI is available. This means that on background tasks you can't access it. But that doesn't mean that you can't access it "outside" of components.

- What are some common use cases for using the Context API?
  - Themes.
  - Multilingual application.
  - Authorisation: setting the user role and info.

## Terms :
- `global state`: provides a way to pass data through the component tree having to pass props down manually at every level, managing state in multiple components that are not directly connected

- `global context`: Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user,

- `provider`: Every Context object comes with a Provider React component that allows consuming components to subscribe to context changes. The Provider component accepts a value prop to be passed to consuming components that are descendants of this Provider. One Provider can be connected to many consumers.

- `onsumer`: A React component that subscribes to context changes. Using this component lets you subscribe to a context within a function component.

## RBAC
Role-based access control (RBAC) restricts network access based on a person's role within an organization and has become one of the main methods for advanced access control. The roles in RBAC refer to the levels of access that employees have to the network.

#### BENEFITS OF RBAC:
- Reducing administrative work and IT support.
- Maximizing operational efficiency.
- Improving compliance.