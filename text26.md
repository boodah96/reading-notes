## Component Based UI

- ##### Name 5 Javascript UI Frameworks (other than React)
- React. 
- Angular. 
- Vue. 
- Ember. 
- Svelte 
- ##### What’s the difference between a framework and a library?
the technical difference between a framework and library lies in a term called inversion of control. When you use a library, you are in charge of the flow of the application. You are choosing when and where to call the library. When you use a framework, the framework is in charge of the flow.

## Term
`Rendering`: is the process of gathering data (if any) and load the associated templates (or just send the output directly). Then apply the gathered data to the associated templates. The final output is sent to the user.
`Templates`: A  website template is a predesigned resource that shows the structure for the comprehensive layout and display features of any website. It is provided by various suppliers to help make Web design a lot easier for designers. A website template is also known as a 
`State`: state is how something is; its configuration, attributes, condition or information content.

# React
- React (also known as React.js or ReactJS) is an open-source, front end, JavaScript library for building user interfaces or UI components. It is maintained by Facebook and a community of individual developers and companies. React can be used as a base in the development of single-page or mobile applications.

- ##### Rendering Elements
- Unlike browser DOM elements, React elements are plain objects, and are cheap to create. React DOM takes care of updating the DOM to match the React elements.
- Applications built with just React usually have a single root DOM node. If you are integrating React into an existing app, you may have as many isolated root DOM nodes as you like.
- To render a React element into a root DOM node, pass both to` ReactDOM.render()`:


```
 const element = <h1>Hello, world</h1>;
ReactDOM.render(element, document.getElementById('root'));
```
- ### Coding JSX
JSX allows us to write HTML elements in JavaScript and place them in the DOM without any createElement()  and/or appendChild() methods.

JSX converts HTML tags into react elements.