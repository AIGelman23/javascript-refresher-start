# JavaScript Refresher

## JavaScript Can Be Executed In Many Environments

1. In the Browser
    JavaScript code can be included in any website. The code then executes inside the browser (i.e., on the machine of the website visitor). 
2. On Any computer
    Thanks to Node.js or Deno, JavaScript code can be executed outside of the browser too. The code then executes directly on the machine.
3. On mobile Devices
    With extra technologies like Capacitor or React Native you can build mobile apps based on JavaScript. The code then executes on the mobile device.

JavaScript can be added in between script tags or by referencing another JavaScript file using the src attribute. 

    <script src="assets/scripts/app.js" defer></script>
    <script src="assets/scripts/app.js" type="module"></script
    
Declaring the type module allows you to use the JavaScript import statement.

React projects always use a build process -- which injects script tags into the HTML for you. 

With React code the code you write is not the code that is executed by the browser. Instead the code is transformed before it's handed off to the browser. 

The package.json lists files and libraries used by a project. The 'react', 'react-dom', and 'react-scripts' packages provide tools to transform React code before it's injected into the browser. 

Development server watches your source code, and adjusts according to changes that are made. 

React Projects Use a Build Process:

Raw, unprocessed React code won't execute in the browser
(JSX is not a default JavaScript feature)

In addition, the code would not be optimized for production (e.g. not minified)

Minification - names of variables, functions are shortened to reduce the amount of JavaScript code. 

React projects require a build process that transforms your code (e.g. create-react-app, vite, etc) -- this build process does not require any custom setup or tweaking.

With type 'module' ES6 availability -- we can export both a variable and or function. If they keywords 'export default' are used than only the value is exported and not the variable or function. With the 'default' added we are saying there is only 1 thing being exported by the file where these keywords are used. 

Without the export default we can use export and just export multiple functions and or variables. We can then import using import {file1, file2, file3}

## There Are Different Types of Values

1. String - Text values, Wrapped with single or double quotes, can also be created with backticks (`)
2. Number - Positive or negative; With decimal point (float) or without it (integer)
3. Boolean - True or false; A simple "Yes" or "No" value type; Typically used in conditions
4. Null & undefined - "There is no value" - undefined: Default if no value was assigned yet; null: Explicitly assigned by developer (reset value)
5. Special Object Value

## Variables Are Data Containers
1. Variable type
2. Variable name
3. Reusability 
4. Readability

## Variable Identifiers Must Follow Certain Rules & Recommendations
1. Must not contain whitespace or special characters (except $ and _)
2. May contain numbers but must not start with a number
3. Must not class with reserved keywords
4. Should use camelCasing
5. Should describe what the "thing" it identifies contains or does
