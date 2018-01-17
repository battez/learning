# React notes

- use Facebook node create react js to setup
- allows very easy project build, esp. if webpack has been problematic to install

## resources learning
- https://egghead.io/courses/the-beginner-s-guide-to-reactjs
- codecadamey course
- Oreilly book "running"
- nice getting going tutorial with architecture and file placing hints https://www.kirupa.com/react/setting_up_react_environment.htm
- mobile: https://www.raywenderlich.com/165140/react-native-tutorial-building-ios-android-apps-javascript 

## motivation
- mobile apps: React Native brings the React paradigm to mobile app development. It’s goal isn’t to write the code once and run it on any platform. The goal is to learn-once (the React way) and write-anywhere. Better than Phone Gap etc. 
- The community has even added tools such as Expo and Create React Native App to help you quickly build React Native apps without having to touch Xcode or Android Studio!


## sublime / IDE
- install Babel sublime plugin
- set .js view > syntax > all as Babel JS and for .jsx files

## commands
- npm start to refresh app
- npm run build to minify and build out app

## components

### Props (properties)
- one can render components as way of interacting
- a component can pass information to another component. Props.
	- A component's props is an object. It holds information about that component.
- Pass info by giving that component an attribute: give it a name
	- pass information that isn't a string,  wrap in curly braces {}, not quotes (as for strings)
- You will often want a component to display the information that you pass:
	- Find the component class that is going to receive that information.
	- Include this.props.name-of-information in that component class's render method's return statement.
- The most common use of props is to pass information to a component, from a different component. 
	- need to export the outgoing component and include an import in the receiving one.
- You can do more with props than just display them. You can also use props to make decisions.
	- The passed-in name is not displayed in either case! The name is used to decide what will be displayed. This is a common technique.
	- e.g. if return X else return Y
- often will pass *functions* as **props**. It is especially common to pass event handler functions.
- this.props.children will return everything in between a component's opening and closing JSX tags.

### event handler functions.

- How do you define an event handler in React?
- as a method on the component class, just like the render method. 
- Almost all functions that you define in React will be defined in this way, as methods in a class.
- naming convention: If you are listening for a "click" event, then you name your event handler handleClick

## JS remarks re: ECMA6 (ES2015) etc
- support: https://medium.freecodecamp.org/you-might-not-need-to-transpile-your-javascript-4d5e0a438ca & https://philipwalton.com/articles/deploying-es2015-code-in-production-today/ 
- https://developer.mozilla.org/en-US/docs/Web/JavaScript
- need to Transpile: Babel etc. The only way to be sure that your ES6 code will work is to convert it to ES5 code before running it in the browser.
- watch out in .js for if/else not setting scope of inner vars!
- With the let keyword, we can scope a variable to any code block. Using let protects the value of the global variable
- e.g. if(true) { let x = 1 ;}
- same with FOR loops, again , use let, e.g. for(let i = 0;)
- added Classes which are more orthodox than the older prorotype for progs from other languages. 
- Strings: With a template, we can create one string and insert the variable values by surround‐ ing them with ${variable}.
- Default parameters are included in the ES6 spec
- With arrow functions, you can create functions without using the function keyword. You also often do not have to use the return keyword.
- **Promises** Promises give us a way to make sense out of asynchronous behavior. 


