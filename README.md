# hw-antra

What is Flux?

Flux is a unidirectional data flow architecture used for building web applications where managing and sharing state across multiple components is necessary. In Flux, the code is structured into views, stores, and dispatchers. Views can subscribe to stores to receive state updates that influence what is rendered. When a view needs to update a state, it does so via the store’s dispatcher functions. Unlike Redux, Flux allows for multiple stores within the application.

What is Redux? How do you use it with React components?

Redux is a JavaScript library that manages global state in an application. While it’s not tied to any specific framework, it’s commonly used with React. To integrate Redux with React, you need to install the react-redux library in addition to Redux itself. The process involves configuring the store, setting up the initial state and reducer functions, and using the Provider component to wrap your entire React application. This makes the Redux store accessible to all React components.

What is a Reducer?

A reducer is a pure function that takes the current state and an action as arguments, and returns a new state object, representing the updated state. In Redux, reducers are supplied when configuring the store, and actions are dispatched to invoke the reducer to update the state.

How do you choose between Context API and Redux for global state management?

For smaller applications with limited state that doesn’t require frequent updates, the Context API is often sufficient. However, if your application has a complex state logic that requires frequent updates, Redux is a better choice due to its scalability and ability to handle more intricate state management needs.

What is Redux Thunk and why would you use it?

Redux Thunk is a middleware that allows you to write action creators that return functions instead of plain objects. This is useful for handling asynchronous operations, such as fetching data from an API, within a Redux dispatch. Thunks can perform side effects and delay the dispatch of an action until after an asynchronous task is completed, making them ideal for complex state updates that shouldn’t be handled within a reducer, which should remain pure. This helps keep your component logic clean and separates concerns effectively.


