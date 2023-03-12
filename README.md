# webpack-cra


Using CRA is both slow and out of date. With the advent of VITE, anyways CRA is losing pupularity. 

Advantages of CRA:
---> With CRA you one need not worry about the nitty gritty details of how the transpiling(conversion of modern javascript specially ES5 & ES6 features to browser understandable JS)
happens or how bundling of the application as one JS file(usually when building for PROD) will happen or how the injection of the script will occur etc. i.e. it provides
ABSTRACTION from the get go and one can proceed directly to development.

Disadvantages of using CRA:
---> Since CRA provides abstraction, a developer is unable to figue out what is running under the hood i.e. what actually is required to run a react application. Also any customization
to the original configuration is not possible.

What is a Javascript Transpiler?
---> A Javascript transcompiler is mainly used to convert ECMAScript 2015+ code into backwards-compatible JavaScript code that can be run by older JavaScript engines. 
It allows web developers to take advantage of the newest features of the language.

What is a module bundler?
--> Module bundlers are the way to organize and combine many files of JavaScript code into one file. 
A JavaScript bundler can be used when your project becomes too large for a single file or when you're working with libraries that have multiple dependencies.

Libraries Used: 
* Babel | transpiler
* Webpack | module bundler
* Webpack-Cli | webpack CLI provides a flexible set of commands for developers to increase speed when setting up a custom webpack project
* Webpack-dev-server | developement server aloows live reload
* Babel-loader | babel loader configuration dictates how certain file types should be processed when loaded
* Babel preset-react | to support react features(by default babel has support for ECMAScript 2015+ JS code) precisely adds support for JSX
* Babel preset-env | allows us to use the latest JS code, without having to manage the latest syntax transformed that are needed by our target environments, also makes the JS bundles smaller
* HTML Webpack Plugin | allows us to inject the bundled js file into our index.html file
