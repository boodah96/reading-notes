## Redux - Asynchronous Actions
 
- How granular should your reducers be?
There should be a separate reducer function for each slice of data. They are combined before being put into the store.
___________________________________________________________________________________________________
- Pro or Con - multiple reducers can “fire” when a commonly named action is dispatched
This is a Con because you may fire off reducers that you did not intend.
__________________________________________________________________________________________________
- Name a strategy for preventing the above
You can use more specific names that represent the reducer and data want to change .
_________________________________________________________________________________________________

##### TERM:
- `store`:A store is an immutable object tree in Redux. A store is a state container which holds the application's state. Redux can have only a single store in your application. Whenever a store is created in Redux, you need to specify the reducer.

- `combined reducers`: It turns out that Redux lets us combine multiple reducers into one that can be passed into createStore by using a helper function named combineReducers . The way we combine reducers is simple, we create one file per reducer in the reducers directory. We also create a file called index. js inside the reducers directory.

____________________________________________________________________________________________________
### Async Logic and Data Fetching REDUX
- Redux’s actions are dispatched synchronously, which is a problem for any non-trivial app that needs to communicate with an external API or perform side effects. Redux also allows for middleware that sits between an action being dispatched and the action reaching the reducers.

- There are two very popular middleware libraries that allow for side effects and asynchronous actions: Redux Thunk and Redux Saga. In this post, you will explore Redux Thunk.

- Thunk is a programming concept where a function is used to delay the evaluation/calculation of an operation.
Redux Thunk is a middleware that lets you call action creators that return a function instead of an action object. That function receives the store’s dispatch method, which is then used to dispatch regular synchronous actions inside the function’s body once the asynchronous operations have been completed.


