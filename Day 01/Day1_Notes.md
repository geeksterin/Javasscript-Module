# What is Javascript
## At the end of the session , You will be able to  :

- Define JavaScript and its purpose.

- Identify key features of JavaScript.
- Explain what Node is and how to install it.
- Execute a JS file with Node.
- Use console.log() to output information to the console.
- Declare and assign values to JavaScript variables.
- Recognize different data types in JavaScript.
- Apply various operators in JavaScript, including the ternary operator.
- Construct control or selection statements using if, else, else-if, and switch.
- Create loops using for, while, and do-while statements.
## What is JavaScript?

1. JavaScript is a high-level, interpreted programming language that is commonly used for web development. It was created in 1995 by Brendan Eich while he was working at Netscape Communications Corporation. JavaScript is often abbreviated as JS, and it is one of the most popular programming languages in the world.

2. _Purpose_ of JavaScript The purpose of JavaScript is to add interactivity and dynamic functionality to web pages. With JavaScript, you can add animations, respond to user actions, validate user input, and manipulate the HTML and CSS of a web page. It is also commonly used on the server-side with Node.js to build scalable web applications.

3. JavaScript Features JavaScript has several key features that make it a popular choice for web development:

**_Interactivity_**

- JavaScript allows you to add interactive elements to web pages, such as dropdown menus, pop-ups, and animations.

**_Lightweight_**:

- JavaScript is a lightweight programming language that can be easily embedded in web pages.

**_Flexibility_**:

- JavaScript can be used on the client-side (in web browsers) and the server-side (with Node.js).

**_Rich library support_**:

- There are numerous JavaScript libraries and frameworks that make it easier to develop web applications.

**_High performance_**:

- Modern JavaScript engines are highly optimized, making JavaScript code run very quickly in web browsers.

## History of javascript
- JavaScript was created by Brendan Eich in 1995 while he was working for Netscape Communications Corporation.
- It was initially named Mocha, then LiveScript, and finally settled on JavaScript.
The language was designed to add interactivity to web pages and respond to user input.
- Microsoft introduced JScript, which caused some compatibility issues, but these were resolved.
- jQuery was released in 2006, making it easier to use JavaScript in web development.
- Other frameworks like AngularJS, React, and Vue.js have gained popularity in recent years.
- Node.js was introduced in 2009, allowing developers to use JavaScript on the server-side.
- JavaScript continues to evolve and is widely used for web development.

## What is Node?

1. **_Node.js_** is an open-source, cross-platform JavaScript runtime environment that allows developers to run JavaScript code outside of a web browser. It is built on the V8 JavaScript engine (which is used by Google Chrome) and provides a way to write server-side applications using JavaScript.

2. **_Installation_** :

- Installation of Node To install Node.js, you can download the installer from the official Node.js website (<https://nodejs.org/en/>). Once the installer is downloaded, run it and follow the on-screen instructions to complete the installation.

3.  **_Executing_** :

- JS File With Node To execute a JavaScript file with Node.js, you can use the command-line interface (CLI). Open a terminal or command prompt and navigate to the directory that contains the JavaScript file. Then, run the following command:

```js
node <name of your js file>
```

4. This will execute the JavaScript file and output any results to the console.






## console.log()

console.log() is a JavaScript function that is used to output data to the console (in web browsers or with Node.js). It takes one or more arguments and prints them to the console. For example:

```js
console.log("Hello, world!");
```

5. This would output the string "Hello, world!" to the console.

## JS variables

A variable in JavaScript is a container for storing data values. You can declare a variable using the var, let, or const keywords. For example:

```js
var name = "John";
let age = 30;
const PI = 3.14;
```

In this example, name is a variable that stores a string, age is a variable that stores a number, and PI is a variable that stores a constant value.

## Data Types

In the previous section, we mentioned a little bit about data types. Data or values have data types. Data types describe the characteristics of data. Data types can be divided into two:

1. Primitive data types
2. Non-primitive data types(Object References)

## Primitive Data Types

Primitive data types in JavaScript include:

1.  Numbers - Integers, floats
2.  Strings - Any data under single quote, double quote or backtick quote
3.  Booleans - true or false value
4.  Null - empty value or no value
5.  Undefined - a declared variable without a value

Non-primitive data types in JavaScript includes:

1. Objects
2. Arrays

Now, let us see what exactly primitive and non-primitive data types mean.
_Primitive_ data types are immutable(non-modifiable) data types. Once a primitive data type is created we cannot modify it.

**Example:**

```js
let word = "JavaScript";
```

If we try to modify the string stored in variable _word_, JavaScript should raise an error. Any data type under a single quote, double quote, or backtick quote is a string data type.

```js
word[0] = "Y";
```

This expression does not change the string stored in the variable _word_. So, we can say that strings are not modifiable or in other words immutable.
Primitive data types are compared by its values. Let us compare different data values. See the example below:

```js
let numOne = 3;
let numTwo = 3;

console.log(numOne == numTwo); // true

let js = "JavaScript";
let py = "Python";

console.log(js == py); //false

let lightOn = true;
let lightOff = false;

console.log(lightOn == lightOff); // false
```

**_Booleans_**

A boolean data type represents one of the two values:_true_ or _false_. Boolean value is either true or false. The use of these data types will be clear when you start the comparison operator. Any comparisons return a boolean value which is either true or false.

**Example: Boolean Values**

```js
let isLightOn = true;
let isRaining = false;
let isHungry = false;
let isMarried = true;
let truValue = 4 > 3; // true
let falseValue = 4 < 3; // false
```

We agreed that boolean values are either true or false.

**_Undefined_**

If we declare a variable and if we do not assign a value, the value will be undefined. In addition to this, if a function is not returning the value, it will be undefined.

```js
let firstName;
console.log(firstName); //not defined, because it is not assigned to a value yet
```

**_Null_**

```js
let empty = null;
console.log(empty); // -> null , means no value
```

**_Numbers_**

```js
var a = 1;
console.log(a); // -> var holding a number data type
```

**_Strings_**

```js
var a = "Geekster";
console.log(a); // -> var holding a string data type
```

## Non-Primitive Data Types

_Non-primitive_ data types are modifiable or mutable. We can modify the value of non-primitive data types after it gets created.
Let us see by creating an array. An array is a list of data values in a square bracket. Arrays can contain the same or different data types. Array values are referenced by their index. In JavaScript array index starts at zero. I.e., the first element of an array is found at index zero, the second element at index one, and the third element at index two, etc.

```js
let nums = [1, 2, 3];
nums[0] = 10;

console.log(nums); // [10, 2, 3]
```

As you can see, an array, which is a non-primitive data type is mutable. Non-primitive data types cannot be compared by value. Even if two non-primitive data types have the same properties and values, they are not strictly equal.

```js
let nums = [1, 2, 3];
let numbers = [1, 2, 3];

console.log(nums == numbers); // false

let userOne = {
  name: "Asabeneh",
  role: "teaching",
  country: "Finland",
};

let userTwo = {
  name: "Asabeneh",
  role: "teaching",
  country: "Finland",
};

console.log(userOne == userTwo); // false
```

Rule of thumb, we do not compare non-primitive data types. Do not compare arrays, functions, or objects.
Non-primitive values are referred to as reference types, because they are being compared by reference instead of value. Two objects are only strictly equal if they refer to the same underlying object.

```js
let nums = [1, 2, 3];
let numbers = nums;

console.log(nums == numbers); // true

let userOne = {
  name: "Asabeneh",
  role: "teaching",
  country: "Finland",
};

let userTwo = userOne;

console.log(userOne == userTwo); // true
```

If you have a hard time understanding the difference between primitive data types and non-primitive data types, you are not the only one. Calm down and just go to the next section and try to come back after some time. Now let us start the data types by number type.

## Operators

**_Assignment operators_**

An equal sign in JavaScript is an assignment operator. It uses to assign a variable.

```js
let firstName = "Asabeneh";
let country = "Finland";
```

**_Arithmetic Operators_**

Arithmetic operators are mathematical operators.

- Addition(+): a + b
- Subtraction(-): a - b
- Multiplication(_): a _ b
- Division(/): a / b
- Modulus(%): a % b
- Exponential(**): a ** b

```js
let numOne = 4;
let numTwo = 3;
let sum = numOne + numTwo;
let diff = numOne - numTwo;
let mult = numOne * numTwo;
let div = numOne / numTwo;
let remainder = numOne % numTwo;
let powerOf = numOne ** numTwo;

console.log(sum, diff, mult, div, remainder, powerOf); // 7,1,12,1.33,1, 64
```

```js
const PI = 3.14;
let radius = 100; // length in meter

//Let us calculate area of a circle
const areaOfCircle = PI * radius * radius;
console.log(areaOfCircle); //  314 m

const gravity = 9.81; // in m/s2
let mass = 72; // in Kilogram

// Let us calculate weight of an object
const weight = mass * gravity;
console.log(weight); // 706.32 N(Newton)

const boilingPoint = 100; // temperature in oC, boiling point of water
const bodyTemp = 37; // body temperature in oC

// Concatenating string with numbers using string interpolation
/*
 The boiling point of water is 100 oC.
 Human body temperature is 37 oC.
 The gravity of earth is 9.81 m/s2.
 */
console.log(
  `The boiling point of water is ${boilingPoint} oC.\nHuman body temperature is ${bodyTemp} oC.\nThe gravity of earth is ${gravity} m / s2.`
);
```

**_Comparison Operators_**

In programming we compare values, we use comparison operators to compare two values. We check if a value is greater or less or equal to other value.

**Example: Comparison Operators**

```js
console.log(3 > 2); // true, because 3 is greater than 2
console.log(3 >= 2); // true, because 3 is greater than 2
console.log(3 < 2); // false,  because 3 is greater than 2
console.log(2 < 3); // true, because 2 is less than 3
console.log(2 <= 3); // true, because 2 is less than 3
console.log(3 == 2); // false, because 3 is not equal to 2
console.log(3 != 2); // true, because 3 is not equal to 2
console.log(3 == "3"); // true, compare only value
console.log(3 === "3"); // false, compare both value and data type
console.log(3 !== "3"); // true, compare both value and data type
console.log(3 != 3); // false, compare only value
console.log(3 !== 3); // false, compare both value and data type
console.log(0 == false); // true, equivalent
console.log(0 === false); // false, not exactly the same
console.log(0 == ""); // true, equivalent
console.log(0 == " "); // true, equivalent
console.log(0 === ""); // false, not exactly the same
console.log(1 == true); // true, equivalent
console.log(1 === true); // false, not exactly the same
console.log(undefined == null); // true
console.log(undefined === null); // false
console.log(NaN == NaN); // false, not equal
console.log(NaN === NaN); // false
console.log(typeof NaN); // number

console.log("mango".length == "avocado".length); // false
console.log("mango".length != "avocado".length); // true
console.log("mango".length < "avocado".length); // true
console.log("milk".length == "meat".length); // true
console.log("milk".length != "meat".length); // false
console.log("tomato".length == "potato".length); // true
console.log("python".length > "dragon".length); // false
```

Try to understand the above comparisons with some logic. Remembering without any logic might be difficult.
JavaScript is somehow a wired kind of programming language. JavaScript code run and give you a result but unless you are good at it may not be the desired result.

As rule of thumb, if a value is not true with == it will not be equal with ===. Using === is safer than using ==. The following [link](https://dorey.github.io/JavaScript-Equality-Table/) has an exhaustive list of comparison of data types.

**_Logical Operators_**

The following symbols are the common logical operators:
&&(ampersand) , ||(pipe) and !(negation).
The && operator gets true only if the two operands are true.
The || operator gets true either of the operand is true.
The ! operator negates true to false and false to true.

```js
// && ampersand operator example

const check = 4 > 3 && 10 > 5; // true && true -> true
const check = 4 > 3 && 10 < 5; // true && false -> false
const check = 4 < 3 && 10 < 5; // false && false -> false

// || pipe or operator, example

const check = 4 > 3 || 10 > 5; // true  || true -> true
const check = 4 > 3 || 10 < 5; // true  || false -> true
const check = 4 < 3 || 10 < 5; // false || false -> false

//! Negation examples

let check = 4 > 3; // true
let check = !(4 > 3); //  false
let isLightOn = true;
let isLightOff = !isLightOn; // false
let isMarried = !false; // true
```

**_Increment Operator_**

In JavaScript we use the increment operator to increase a value stored in a variable. The increment could be pre or post increment. Let us see each of them:

1. Pre-increment

```js
let count = 0;
console.log(++count); // 1
console.log(count); // 1
```

1. Post-increment

```js
let count = 0;
console.log(count++); // 0
console.log(count); // 1
```

We use most of the time post-increment. At least you should remember how to use post-increment operator.

**_Decrement Operator_**

In JavaScript we use the decrement operator to decrease a value stored in a variable. The decrement could be pre or post decrement. Let us see each of them:

1. Pre-decrement

```js
let count = 0;
console.log(--count); // -1
console.log(count); // -1
```

2. Post-decrement

```js
let count = 0;
console.log(count--); // 0
console.log(count); // -1
```

**_Ternary Operators_**

Ternary operator allows to write a condition.
Another way to write conditionals is using ternary operators. Look at the following examples:

```js
let isRaining = true;
isRaining
  ? console.log("You need a rain coat.")
  : console.log("No need for a rain coat.");
isRaining = false;

isRaining
  ? console.log("You need a rain coat.")
  : console.log("No need for a rain coat.");
```

```sh
You need a rain coat.
No need for a rain coat.
```

```js
let number = 5;
number > 0
  ? console.log(`${number} is a positive number`)
  : console.log(`${number} is a negative number`);
number = -5;

number > 0
  ? console.log(`${number} is a positive number`)
  : console.log(`${number} is a negative number`);
```

```sh
5 is a positive number
-5 is a negative number
```

## Conditionals

Conditional statements are used for make decisions based on different conditions.
By default , statements in JavaScript script executed sequentially from top to bottom. If the processing logic require so, the sequential flow of execution can be altered in two ways:

- Conditional execution: a block of one or more statements will be executed if a certain expression is true
- Repetitive execution: a block of one or more statements will be repetitively executed as long as a certain expression is true. In this section, we will cover _if_, _else_ , _else if_ statements. The comparison and logical operators we learned in the previous sections will be useful in here.

Conditions can be implementing using the following ways:

- if
- if else
- if else if else
- switch
- ternary operator

**_If_**

In JavaScript and other programming languages the key word _if_ is to used check if a condition is true and to execute the block code. To create an if condition, we need _if_ keyword, condition inside a parenthesis and block of code inside a curly bracket({}).

```js
// syntax
if (condition) {
  //this part of code runs for truthy condition
}
```

**_Example:_**

```js
let num = 3;
if (num > 0) {
  console.log(`${num} is a positive number`);
}
//  3 is a positive number
```

As you can see in the condition example above, 3 is greater than 0, so it is a positive number. The condition was true and the block of code was executed. However, if the condition is false, we won't see any results.

```js
let isRaining = true;
if (isRaining) {
  console.log("Remember to take your rain coat.");
}
```

The same goes for the second condition, if isRaining is false the if block will not be executed and we do not see any output. In order to see the result of a falsy condition, we should have another block, which is going to be _else_.

**_If Else_**

If condition is true the first block will be executed, if not the else condition will be executed.

```js
// syntax
if (condition) {
  // this part of code runs for truthy condition
} else {
  // this part of code runs for false condition
}
```

```js
let num = 3;
if (num > 0) {
  console.log(`${num} is a positive number`);
} else {
  console.log(`${num} is a negative number`);
}
//  3 is a positive number

num = -3;
if (num > 0) {
  console.log(`${num} is a positive number`);
} else {
  console.log(`${num} is a negative number`);
}
//  -3 is a negative number
```

The last condition is false, therefore the else block was executed. What if we have more than two conditions? In that case, we would use _else if_ conditions.

**_If Else if Else_**

On our daily life, we make decisions on daily basis. We make decisions not by checking one or two conditions instead we make decisions based on multiple conditions. As similar to our daily life, programming is also full of conditions. We use _else if_ when we have multiple conditions.

```js
// syntax
if (condition) {
  // code
} else if (condition) {
  // code
} else {
  //  code
}
```

**Example:**

```js
let a = 0;
if (a > 0) {
  console.log(`${a} is a positive number`);
} else if (a < 0) {
  console.log(`${a} is a negative number`);
} else if (a == 0) {
  console.log(`${a} is zero`);
} else {
  console.log(`${a} is not a number`);
}
```

\***\*Switch\*\***

Switch is an alternative for **if else if else else**.
The switch statement starts with a _switch_ keyword followed by a parenthesis and code block. Inside the code block we will have different cases. Case block runs if the value in the switch statement parenthesis matches with the case value. The break statement is to terminate execution so the code execution does not go down after the condition is satisfied. The default block runs if all the cases don't satisfy the condition.

```js
switch (caseValue) {
  case 1:
    // code
    break;
  case 2:
    // code
    break;
  case 3:
    // code
    break;
  default:
  // code
}
```

```js
let weather = "cloudy";
switch (weather) {
  case "rainy":
    console.log("You need a rain coat.");
    break;
  case "cloudy":
    console.log("It might be cold, you need a jacket.");
    break;
  case "sunny":
    console.log("Go out freely.");
    break;
  default:
    console.log(" No need for rain coat.");
}
```

// Examples to use conditions in the cases

```js
let num = prompt("Enter number");
switch (true) {
  case num > 0:
    console.log("Number is positive");
    break;
  case num == 0:
    console.log("Numbers is zero");
    break;
  case num < 0:
    console.log("Number is negative");
    break;
  default:
    console.log("Entered value was not a number");
}
```

**_Ternary Operators_**

Another way to write conditionals is using ternary operators. We have covered this in other sections, but we should also mention it here.

```js
let isRaining = true;
isRaining
  ? console.log("You need a rain coat.")
  : console.log("No need for a rain coat.");
```

More Examples - https://www.programiz.com/javascript/ternary-operator

## Loops

**_For loop_**

The for loop is the most common loop used in JavaScript. It consists of three parts:

Initialization of a variable (usually an index variable) to a starting value
A condition that is checked before each iteration of the loop
An update to the index variable at the end of each iteration
The syntax for a for loop is as follows:

```js
for (var i = 0; i < 5; i++) {
  console.log(i);
}
```

In the example above, the for loop initializes the variable i to 0, checks the condition that i is less than 5 before each iteration, and updates i by incrementing it by 1 after each iteration.

Example 1: Printing numbers from 1 to 10 using for loop:

```js
for (let i = 1; i <= 10; i++) {
  console.log(i);
}
```

In this example, we are using a for loop to iterate over the numbers from 1 to 10. The initialization statement let i = 1 sets the starting value of the loop counter variable to 1. The condition i <= 10 checks if the loop counter variable is less than or equal to 10. The increment statement i++ increases the loop counter variable by 1 after each iteration. The loop will execute 10 times, with the loop counter variable taking on values from 1 to 10.

**_while loop_**

The while loop is used when the number of iterations is unknown, and the loop continues as long as a specified condition is true. The syntax for a while loop is as follows:

```js
var i = 0;
while (i < 5) {
  console.log(i);
  i++;
}
```

In the example above, the while loop continues as long as i is less than 5, and i is incremented by 1 after each iteration.
More example: Printing numbers from 1 to 10 using while loop

```js
let i = 1;

while (i <= 10) {
  console.log(i);
  i++;
}
```

In this example, we are using a while loop to iterate over the numbers from 1 to 10. The initialization statement let i = 1 sets the starting value of the loop counter variable to 1. The condition i <= 10 checks if the loop counter variable is less than or equal to 10. The increment statement i++ increases the loop counter variable by 1 after each iteration. The loop will execute 10 times, with the loop counter variable taking on values from 1 to 10.

**_do-while loop_**

The do-while loop is similar to the while loop, but it executes the code block at least once before checking the condition. The syntax for a do-while loop is as follows:

```js
var i = 0;
do {
  console.log(i);
  i++;
} while (i < 5);
```

In the example above, the do-while loop executes the code block once before checking the condition that i is less than 5. If the condition is true, the loop continues executing until the condition is false.

More example : Printing numbers from 1 to 5 using do-while loop

```js
let i = 1;

do {
  console.log(i);
  i++;
} while (i <= 5);
```

In this example, we are using a do-while loop to print numbers from 1 to 5. The do block contains the code that prints the value of the i variable to the console and increments the value of i by 1. The while block contains the condition that checks if the value of i is less than or equal to 5. If the condition is true, the loop will execute again, printing the next number until the value of i becomes 6 and the condition becomes false, at which point the loop will exit.

# Class Assignment (to be done in class)

1. [Chaining If Else Statements](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/chaining-if-else-statements)

2. [Selecting from Many Options with Switch Statements](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/selecting-from-many-options-with-switch-statements)

3. [Adding a Default Option in Switch Statements](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/adding-a-default-option-in-switch-statements)

4. [Multiple Identical Options in Switch Statements](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/multiple-identical-options-in-switch-statements)
