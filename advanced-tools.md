## Redux
Redux is a state manager library, it has an official integration with React, called [React-Redux](https://react-redux.js.org/), to learn more about this library you will dive through it's fundamentals with the maker of this tool, Dan Abramov, the tutorial is available [here](https://egghead.io/courses/fundamentals-of-redux-course-from-dan-abramov-bd5cc867).

The objectives for this tutorial are:
- Learn how to add proper state management to your React app;
- Dive through reducers and how to manipulate state changes;
- How to propagate the changes into the components;
- Make a To-do list using this library;
  
## Tools
To get a react app setup, there's some background work that still has to be done like setting up a webpack dev server, configuring your babel transpiler, etc. To make our lifes easier there are already tools that do this out of the box, but in order to use it, it helps understanding what they do. Apart from this setup shenanigans, in a real environment having your code supported by tests will help you preventing major code breaking releases. 

[Here](https://www.tutorialspoint.com/babeljs/babeljs_working_babel_with_webpack.htm) you'll learn more about what Babel does and why do we need to setup webpack.

After understanding the fundamentals and see the amount of boilerplate code it is needed, we introduce the `create-react-app` tool, this tool brings all the basic configuration that a react app needs to in order to be up and running. You can learn how to use it [here](https://github.com/facebook/create-react-app)

[Here](https://jkettmann.com/beginners-guide-to-testing-react) you'll dive into the React testing world, you'll learn how to mock api calls and even mock user interactions (clicking a button or typing on an input).

Objectives for these tutorials:
- Learn more about Babel and Webpack;
- See how to create a react project in one minute;
- Learn how to test:
  - Mock User interactions;
  - Mock API Calls;
  - Mock page rendering;

## Next.js
Next.js is a framework that brings Server-Side Rendering, typescript support and even route handling to your react app out of the box with no need for importing more and more packages in order to add these features to your app. This will serve as the last tool you'll learn from our onboarding since this will use all of the concepts that were shown previously.

With this [guide](https://nextjs.org/learn/basics/create-nextjs-app), you'll learn:
- How to setup a next.js app;
- Add routing based on your file system routing;
- Migrating an app from Javascript to Typescript;
