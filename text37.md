
#  Redux - Combined Reducers
- Why choose Redux instead of the Context API for global state?
Redux is the industry standard for managing state of large applications, so it is important to know well. It is more optimized for larger projects, because the context API re-renders more often.


____________________________________________________________________
- What is the purpose of a reducer?
A reducer is a function that determines changes to an application's state. It uses the action it receives to determine this change. We have tools, like Redux, that help manage an application's state changes in a single store so that they behave consistently.

_________________________________________________________________________
-  What does an action contain?
An action contains a type and whatever payload you want it to have.


_______________________________________________________________________________
- Why do we need to copy the state in a reducer?
The reducer needs to be a pure function without any side-effects. It should only take in an action and return the new state.

____________________________________________________________________________

## TERMS:
- `immutable state`: Immutable state is state that cannot be changed. Immutable objects (for which none of the state can be changed) become important when you are dealing with concurrency, the ability for more than one processor in your computer to operate on that object at the same time.

- `time travel in redux`: The Redux DevTools records dispatched actions and the state of the Redux store at every point in time. ... This makes it possible to inspect the state and travel back in time to a previous application state without reloading the page or restarting the app.

- `action creator`: An action creator is merely a function that returns an action object. Redux includes a utility function called bindActionCreators for binding one or more action creators to the store's dispatch() function.

- `reducer`: Reducers tell the application how to change state in response to an action. dispatch This is the name of the function you use to send actions to the store.

- `dispatch`: dispatch is a function of the Redux store. You call store. dispatch to dispatch an action. This is the only way to trigger a state change. With React Redux, your components never access the store directly - connect does it for you.

__________________________________________________________________________
## Using combineReducers:

- The combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore .
- reducers (Object): An object whose values correspond to different reducing functions that need to be combined into one. See the notes below for some rules every passed reducer must follow.

- The resulting reducer calls every child reducer and gathers their results into a single state object.

- combineReducers will combine all the reducers passed to it into a single reducing function