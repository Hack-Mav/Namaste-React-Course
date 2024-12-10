# Assignemnt

## What is Emmet?
Emmet is a powerful and widely-used toolkit for web developers that help to speed up writing HTML and CSS. It allows you to write shorthand code (called Emmet abbreviations) that gets expanded into full-fledged HTML or CSS. The purpose of Emmet is to help you write code faster, more efficiently, and with fewer errors.

## Difference between a Library and Framework?
The term Library and Framework are often used interchangeably in programming, but they have distinct differences.

### 1. Definition
  - Library: A library is a collection of pre-written code, functions, classes, and routines that you can use to perform common tasks. It provides specific functionality that you can call and use as needed, but you maintain full control over the flow of your application.

  - Framework: A framework is a more extensive, larger collection of code that provides a foundation for building software applications. It dictates the structure and flow of your application and often enforces rules on how you should organize your code. In a framework, the control flow is typically inverted, meaning the framework call your code, not the other way around.

### 2. Examples

  - Library Examples:
    - jQuery: A JavaScript library for DOM manipulation.
    - Lodash: A utility library for JavaScript that simplifies common programming tasks (e.g., manipulating arrays, objects, etc.).
    - NumPy: A Python library for scientific computing that provides support for large arrays and matrices.

  - Framework Examples:
    - React: A JavaScript framework for building user interfaces. It dictates how your components should be structured and how state and rendering should work.
    - Django: A Python framework for building web applications that provides an ORM, templates, and a robust way to manage web projects.
    - Angular: A framework for building single-page web applications that provides tools like routing, dependency injection, and state management.


##  What is CDN? Why do we use it?
A Content Delivery Network (CDN) is a system of geographically distributed servers designed to deliver content (such as web pages, images, videos, JavaScript, stylsheets, etc.) to users based on their geographical location. The primary goal of a CDN is to speed up the delivery of content by reducing latency and minimizing the distance between the user and the server hosting the content.

A CDN typically works by replicating content across multiple servers located in different regions or data centers around the world. When a user requests content, the CDN will route that request to the closest available server, thereby reducing the time it take for the content to reach the user.

CDNs offer several benefits, especially for websites and applications that serve large amounts of content or have global audiences. Here are the key reasons to use a CDN:
1. Improved Performance and Speed
2. Scalability
3. Reduced Bandwidth Costs
4. Improved Avaliability and Reliability 
5. Security Benefits
6. SEO Benefits
7. Global Reach


##  Why is React known as React? 
React is known as "React" because the library is built around the concept of reactivity---it "reacts" to changes in data and updates the user interface accordingly. The name emphasizes the core functionality of the library, which is to react to changes in the state of the application and efficiently render updates to the view.    


##  What is crossorigin in script tag? 
The ```crossorigin``` attribute in the ```<script>``` tag is used to control how the browser handles cross-origin requests for scripts, particularly in situations where a script is loaded from a different domain (a cross-origin request). It is important for managing **CORS (Cross-Origin Resource Sharing)** policies, which control how resources from different origins can be accessed.

The ```crossorigin``` attribute can take three possible values:
1. ```anonymous``` (default behaviour)
2. ```use-credentials```
3. No ```crossorigin``` attribute


## What is diference between React and ReactDOM


| **Feature**           | **React**                                       | **ReactDOM**                                              |
|-----------------------|-------------------------------------------------|-----------------------------------------------------------|
| **Core Purpose**      | Provides the core functionality of React        | Provides DOM-specific methods to render and manage the    |
|                       | (components, JSX, state management, etc.)       | DOM in a web environment                                  |
|-----------------------|-------------------------------------------------|-----------------------------------------------------------|
| **Primary Role**      | Defines the structure, logic, and behavior of   | Renders React components to the DOM                       |
|                       | UI components                                   |                                                           |
|-----------------------|-------------------------------------------------|-----------------------------------------------------------|
| **Usage**             | Used in both web and non-web (e.g., React Native)| Specifically used for rendering in web browsers          |
|                       | environments                                    |                                                           |
|-----------------------|-------------------------------------------------|-----------------------------------------------------------|
| **Key Methods**       | `React.createElement()`, `React.Component`, JSX | `ReactDOM.render()`, `ReactDOM.hydrate()`                 |
|-----------------------|-------------------------------------------------|-----------------------------------------------------------|
| **Environment**       | Can be used in any JavaScript environment (e.g.,| Used exclusively in the browser environment               |
|                       | React Native, server-side rendering, etc.)      |                                                           |
|-----------------------|-------------------------------------------------|-----------------------------------------------------------|


## What is the difference between `react.development.js` and `react.production.js` files via CDN?

| **Feature**           | **react.development.js**                                      | **react.production.min.js**                                      |
|-----------------------|---------------------------------------------------------------|-------------------------------------------------------------------|
| **Purpose**           | Development (debugging, error handling, verbose messages)      | Production (optimized, faster execution, smaller size)            |
| **File Size**         | Larger due to extra debugging code, unminified                 | Smaller, minified, with no debugging code                         |
| **Performance**       | Slower (extra checks and verbose error messages)               | Faster, optimized for performance                                |
| **Debugging**         | Includes helpful warnings, error messages, and debugging info  | No debugging features, only the core React functionality          |
| **Error Handling**    | More verbose and helpful error messages for developers         | Error handling is stripped down to increase performance           |
| **Use Case**          | Best for development and testing                              | Best for production environments where performance is crucial     |


##  What is async and defer?
In the context of HTML ```<script>``` tags, ```async``` and ```defer``` are attributes that control how external JavaScript files are loaded and executed in relation to the HTML document. These attributes help improve the performance of web pages by controlling the timing of script execution.

1. ```async``` Attribute
The ```async``` attribute is used to load and execute the script asynchronously. This means that the script is fetched and executed in parallel with the parsing of the HTML document, without blocking the rendering of the page.

2. ```defer``` Attribute
The ```defer``` attribute is used to load the script asynchronously, but with one key difference: the script is **executed only after the HTML document has been fully parsed**. This ensures that the script is executed after the document is completely ready, without blocking the HTML parsing.