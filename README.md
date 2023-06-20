# JavaScriptWithCommonJS-Sample1

CommonJS is a module system used in JavaScript for organizing and structuring code. It allows you to define modules using the module.exports syntax and import them using the require function. Here's an example of a JavaScript application using CommonJS:

Let's say we want to create a simple application that calculates the square of a number. We'll create two files: calculator.js and index.js.

In calculator.js, we'll define a module that exports a function to calculate the square of a number:

```javascript
// calculator.js
function square(num) {
  return num * num;
}

module.exports = square;
```

In index.js, we'll import the square function from the calculator module and use it:

```javascript
// index.js
const square = require('./calculator');

const result = square(5);
console.log(result); // Output: 25
```

Now, to run this project in VSCode, follow these steps:

1.Open VSCode and create a new folder for your project.

2.Inside the project folder, create the calculator.js and index.js files with the respective code as mentioned above.

3.Open a terminal in VSCode by going to View -> Terminal.

4.Make sure you have Node.js installed on your machine. You can check by running node -v in the terminal. 

If it's not installed, download and install it from the official Node.js website.

5.In the terminal, navigate to your project folder using the cd command. For example: 
```
cd path/to/your/project/folder.
```

6.Once you're inside the project folder, run the following command in the terminal: 
```
node index.js.
```

7.You should see the output 25 printed in the terminal, which is the result of the square calculation.

That's it! You've successfully created and run a JavaScript application using CommonJS in VSCode.
