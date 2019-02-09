1.  Name 3 JavaScript Array/Object Methods that do not produce side-effects? Which method do we use to create a new object while extending the properties of another object?
map, reduce, Object.create/Object.assign

1.  Describe `actions`, `reducers` and the `store` and their role in Redux. What does each piece do? Why is the store known as a 'single source of truth' in a redux application?
Actions are just functions that pass data from store to app. Reducers are change state in reponse to actions. Store is where the state lives and it's accessible without having to pass through all the parent components. 
1.  What is the difference between Application state and Component state? When would be a good time to use one over the other?
Application state is globe and while component state is local. Good time to use it is when data needs to be passed between components then we use global state. 
1.  What is middleware?
Middleware basically is a chunk of code that allows us to use as a way to interact with actions before they reach the reducer, for something like logging or changing the action. 
1.  Describe `redux-thunk`, what does it allow us to do? How does it change our `action-creators`?
it's a middleware that lets you call action creators and return a function instead of an action object. That funcion receives store's dispatch method, which is then used to dispatch regular async actions & inside body of that func. once the async operations have completed. 
1.  Which `react-redux` method links up our `components` with our `redux store`?
connect()()
