# Props and State

- Does a deployed React application require a server?
You don't necessarily need a static server in order to run a Create React App project in production. It also works well when integrated into an existing server side app.


- Why do we prefer to test a React application at the behavior rather than the unit level?

teration speed vs Realistic environment: Some tools offer a very quick feedback loop between making a change and seeing the result, but don’t model the browser behavior precisely. Other tools might use a real browser environment, but reduce the iteration speed and are flakier on a continuous integration server.

- What does npm run build do?

runs the script "build" and created a script which runs your application


- Describe the actual composition / architecture of a React application
Unlike other UI libraries and frameworks, Reactjs doesn’t enforce an architecture pattern. It is just a view that caters to the user interface. Just beneath the user interface lies a tree of several React components.
## TERM
`BDD`: behavior-driven development is an Agile software development process that encourages collaboration among developers, QA, and non-technical or business participants in a software project. It encourages teams to use conversation and concrete examples to formalize a shared understanding of how the application should behave.

`Acceptance Tests`: An acceptance test is a formal description of the behavior of a software product, generally expressed as an example or a usage scenario. A number of different notations and approaches have been proposed for such examples or scenarios. In many cases the aim is that it should be possible to automate the execution of such tests by a software tool, either ad-hoc to the development team or off the shelf.

`mounting`: Mounting is a process by which the operating system makes files and directories on a storage device (such as hard drive, CD-ROM, or network share) available for users to access via the computer’s file system.

`build`: The term build may refer to the process by which source code is converted into a stand-alone form that can be run on a computer or to the form itself. One of the most important steps of a software build is the compilation process, where source code files are converted into executable code.

## setState :
- setState() is the only legitimate way to update state after the initial state setup. Let’s say we have a search component and want to display the search term a user submits.

* Update to a component state should be done using setState()

- You can pass an object or a function to setState()

* Pass a function when you can to update state multiple times

- Do not depend on this.state immediately after calling setState() and make use of the updater function instead.

### Handling Events:
- React events are named using camelCase, rather than lowercase.

- With JSX you pass a function as the event handler, rather than a string.

- you cannot return false to prevent default behavior in React. You must call preventDefault explicitly.

