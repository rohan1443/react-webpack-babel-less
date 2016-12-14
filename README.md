# react-webpack-babel-less
https://github.com/rohan1443/react-webpack-babel-less.git
Simple React Webpack Babel Less Starter Kit

Tired of complicated starters with 200MB of dependencies which are hard to understand and modify?

Try this is a simple [React](https://facebook.github.io/react/), [Webpack](http://webpack.github.io/) and [Babel](https://babeljs.io/) application with nothing else in it.

### What's in it?

* Simple src/index.jsx and src/index.css (local module css).
* Webpack configuration for development (with hot reloading) and production (with minification).
* CSS module loading, so you can include your css by ```import styles from './path/to.css';```.
* Both js(x) and css hot loaded during development.

### To run

* You'll need to have [git](https://git-scm.com/) and [node](https://nodejs.org/en/) installed in your system.
* Fork and clone the project:

```
git clone https://github.com/rohan1443/react-webpack-babel-less.git
```

* Then install the dependencies:

```
npm install
```

* Run development server:

```
npm start
```

Open the web browser to `http://localhost:8888/`

### To build the production package

```
npm run build
```

Below configuration and settings are optional




### Definitions To Know 

#### babel plugin transform decorators legacy :- compile class and object decorators to ES5

#### babel plugin transform class properties :- This plugin transforms static class properties as well as properties declared with the property initializer syntax

#### babel plugin transform runtime :- Externalise references to helpers and builtins, automatically polyfilling your code without polluting globals

#### babel-runtime :- self contained runtime

### css-loader :- 
Example - 
var css = require("css-loader!./file.css");
// => returns css code from file.css, resolves imports and url(...) 
(can use require(...) for loading the css file via lazy loading instead of using import or url(...))




### Eslint
There is a .eslint.yaml config for eslint ready with React plugin.
To use it, you need to install additional dependencies though:

```
npm install --save-dev eslint eslint-plugin-react
```

To do the actual linting, run:

```
npm run lint
```


### Notes on importing css styles
* styles having /src/ in their absolute path are considered part of the application and exported as local css modules.
* other styles are considered global styles used by many components and are included in the css bundle directly.

### Contribute
Please contribute to the project if you know how to make it better, including this README :)
