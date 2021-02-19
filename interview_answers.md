# Interview Answers
Be prepared to demonstrate your understanding of this week's concepts by answering questions on the following topics. These will not be counted as a part of your sprint score but will be helpful for preparing you for your endorsement interview, and enhancing overall understanding.

1. What problem does the context API help solve?

    The problem of cumbersome prop drilling in larger applications. When we have global state which many components share, it can become especially cumbersome to need to consistently pass said data down through props - not to mention messy! Using Context API in such a case can eliminate prop drilling altogether if so desired, and helps to produce cleaner, more readable, more easily managed code & state/data.

2. In your own words, describe `actions`, `reducers` and the `store` and their role in Redux. What does each piece do? Why is the store known as a 'single source of truth' in a redux application?

    1. Actions: Actions are like the director in the action/reducer one-two punch - they dictate when and how the reducers need to update state.
    2. Reducers: If actions are the director, reducers are the actors - they take direction through action types and payloads and use that direction to know when, where, and how to update our state.
    3. Store: Continuing this analogy, I suppose you could say the store is like the studio - It's the piece of the loop that links our state, reducers, and actions to our App, while our App connects to it. The store is our singular source of truth for the rest of our application and ties the whole package together.

3. What does `redux-thunk` allow us to do? How does it change our `action-creators`?

    Redux-Thunk allows us to utilize our action creators to perform asynchronous actions/functions/operations with our action creators. Because the Redux action -> reducer flow is by nature synchronous, this is vital for allowing our actions to do things like make API calls to receive data and update our state accordingly.

    They can also change our action reducers in the form of allowing us to combine all of our action creators into one single thunk-function package, which can simplify things greatly if implemented correctly.

4. What is your favorite state management system you've learned and this sprint? Please explain why!

    Definitely Redux! Context API is nice because it's lightweight in nature, taking less boilerplate and initial setup, but in my opinion I feel as though the entire Redux system/workflow gives way to much more functionality and nuance for our applications. It's also just a joy to work with!

    That being said, I enjoy the idea of using a combination of both over my career for different purposes - Context API for smaller, simpler applications, and Redux for larger, more robust applications.