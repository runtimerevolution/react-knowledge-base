# React.js for beginner
<img src="assets/react.png" align="right" style="width: 200px; margin-left: 20px;"/>

## Table of contents
1. [What is React.js](#atom_symbol-what-is-reactjs)
2. [Getting Started](#rocket-getting-started)
3. [React Hooks](#hook-react-hooks)
4. [React Router](#arrow_right_hook-react-router)
5. [Build your first app](#technologist-build-your-first-app)

<br/>

## :atom_symbol: What is React.js

`React.js` is an open-source JavaScript library that is used for building user interfaces specifically for single-page applications.

It was first created by Jordan Walke, a software engineer working for Facebook, and is now one of the most commonly used frontend libraries for web development.

Although React is a library rather than a language, it is widely used in web development since it allows developers to create large web applications that are constantly refreshing data in the UI. This technology eliminates the need of reloading the whole screen and also avoids processing every single line of code.

__The main purpose of React is to be fast, scalable, and simple.__

## :rocket: Getting Started

### The official documentation
There is no better way to get started in React.js than the official documentation. [Here](https://reactjs.org/docs/hello-world.html) you will find a brief description of the main concepts as well as links to CodePen where you can change the code and see what it does in real time. The goal here is for you to start think in React.

### The Beginner's Guide to React
Once you're done with the official documentation it's time to build a solid foundation with [The Beginner's Guide to React](https://egghead.io/courses/the-beginner-s-guide-to-react). It is a 28-part course with short lessons where you'll learn many interesting think like how to:

* What is JSX and how to use it effectively with React
* Create simple and reusable React components
* Style React components with className and inline Styles
* What are hooks and how to create your own
* Make and manage basic forms
* Make HTTP requests
* Install and use React DevTools for debugging
* Build and deploy a React Application with Codesandbox, GitHub, and Netlify

## :hook: React Hooks

Hooks are a feature introduced in the React 16.8 version. It provides an alternative to writing class-based components, and offers an alternative approach to state management and lifecycle methods.

Since they were already introduced in the [The Beginner's Guide to React](#the-beginners-guide-to-react) we give you two suggestions on how to expand your knowledge in this subject:

1. Go trough the [official documentation](https://reactjs.org/docs/hooks-intro.html) for an overview of how the hook work (or experienced React users)
2. Learn how they work in a more in-depth way with the [Build Advanced Components with React Hooks](https://egghead.io/courses/build-advanced-components-with-react-hooks-810906cc) course where you will learn how to:
    * Manage React component state with useState
    * Share values throughout an application with Context
    * Build a React compound component
    * Render multiple pages in a Wizard form
    * Handle complex state updates with useReducer

## :arrow_right_hook: React Router

Even tough React is built for single-page applications we can still build apps with multiple routes using [React Router](https://reactrouter.com/). It that allows you to handle routes in a web app, using _dynamic routing_,  meaning routing that takes place as your app is rendering, not in a configuration or convention outside of a running app. That means almost everything is a component in React Router.

A great way to learn about React Router is using the [official tutorial](https://reactrouter.com/docs/en/v6/getting-started/tutorial) that will cover the following topics:

* Configuring Routes
* Navigating with Link
* Creating Links with active styling
* Using Nested Routes for Layout
* Navigating programmatically
* Using URL params for data loading
* Using URL Search params
* Creating your own behaviors through composition
* Server Rendering

## :technologist: Build your first app

<img src="assets/react2.png" align="right" style="width: 200px; margin-left: 20px;"/>

That that you have learn the basics of React.js, it's time to create your first app. Here we are going to use the [API](https://www.themoviedb.org/documentation/api) for The Movie Data Base (TMDB) to get data and show it in our application but you can use any API you prefer. Here is a list of public API's: https://github.com/public-apis/public-apis

With the TMDB we can create movie database app, where the user can search for movies, TV shows and crew members.

Since making CSS is not the goal here, we recommend you use a package with pre-made CSS components:
* [Bootstrap](https://react-bootstrap.github.io/)
* [Material UI](https://mui.com/pt/)

Here is our suggestion on where to start.

### 1. Request an API key
The API is free and available for everyone to use but in order to make request you need to create a user account and then [request an API key](https://www.themoviedb.org/settings/api).

### 2. Create the home page
This is the first page the user will see in your application. Here you can have show the 5 [most popular movies](https://developers.themoviedb.org/3/movies/get-popular-movies) as well as an input to allow the user to search by TV shows, movies or people using these endpoints:
* TV Shows: https://developers.themoviedb.org/3/search/search-tv-shows
* Movies: https://developers.themoviedb.org/3/search/search-movies
* People: https://developers.themoviedb.org/3/search/search-people

After clicking the search button — and if there is something to search for —, the user should be redirected to another page where the search results will appear (5 for each category is enough).

### 3. TV Show page
This is the page for the TV Show. Here you can use the URL params to get the TV show ID and show the following:
* Details: https://developers.themoviedb.org/3/tv/get-tv-details
* Credits: https://developers.themoviedb.org/3/tv-seasons/get-tv-season-aggregate-credits

### 4. Movie page
This is the page for the movie. Here you can use the URL params to get the movie ID and show the following:
* Details: https://developers.themoviedb.org/3/movies/get-movie-details
* Credits: https://developers.themoviedb.org/3/movies/get-movie-credits

### 5. Person page
This is the page for a person. Here you can use the URL params to get the person ID and show the following:
* Details https://developers.themoviedb.org/3/people/get-person-details
* TV shows: https://developers.themoviedb.org/3/people/get-person-tv-credits
* Movies: https://developers.themoviedb.org/3/people/get-person-movie-credits

### 6. Connection everything
Now that we have a specific page for everything we just need to add links so that, in the search results page, when a user click a result they are redirected to the specific page. Same thing for the credits, they should redirect to the correct person page.

### 7. Bonus
As a bonus, and if the rest was too easy for you, you can use the knowledge acquired in the previous steps to deploy your app and show it off. 🚀


## The end

Congratulations! 🎉 You have completed the beginners guide to React.js. This is the end of this chapter but the beginning of your journey with React.js so fell free to go back to the [start](/README.md) and learn more. After all, it's a never end story...

<p align="center">
    <img src="https://i.giphy.com/9oEclSzXUfh5u.gif"/>
</p>
