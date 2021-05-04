# Component Composition

1- Can a parent component access the state of a child component?
In React we can access the child's state using Refs. we will assign a Refs for the child component in the parent component. then using Refs we can access the child's state. Creating Refs Refs are created using React.

2- What can be passed along in a prop variable?

props enable you to pass variables from one to another component down the component tree. In the previous example, it was only a string variable. But props can be anything from integers over objects to arrays.

3-How can a child component “know” the state of another component?

The most common method is to make a callback function that the child component will trigger and toss the state values upward.

### TERMS

`component props`: Properties which is object argument that conatains data or functions.

`component state`: The state is an instance of React Component Class can be defined as an object of a set of observable properties that control the behavior of the component. In other words, the State of a component is an object that holds some information that may change over the lifetime of the component.

`application state`: In the simplest terms, it is a JavaScript object that represents the part of a component that can change

#### React Basic Mounting

Since class-based components are classes, hence the name, the first method that runs is the constructor method. Typically, the constructor is where you would initialize component state.

Next, the component runs the getDerivedStateFromProps. I’m going to skip this method since it has limited use.

Now we come to the render method which returns your JSX. Now React “mounts” onto the DOM.



#### Updating

This phase is triggered every time state or props change. Like in mounting, getDerivedStateFromProps is called (but no constructor this time!).

Next shouldComponentUpdate runs. Here you can compare old props/state with the new set of props/state. You can determine if your component should re-render or not by returning true or false. This can make your web app more efficient by cutting down on extra re-renders. If shouldComponentUpdate returns false, this update cycle ends.

If not, React re-renders and getSnapshotBeforeUpdate runs afterwards. This method has limited use as well. React then runs componentDidUpdate. Like componentDidMount you can use it to make any async calls or manipulate the DOM.