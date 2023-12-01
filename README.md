# Day 1

![day-one-image](./images/dayOne.jpg)

Today I have learned:

- There are 7 types of data that are meaningful to the computer: number
- Using assignment operator to give values to variables
- When the variables are first declared, they are initialized with the value of undefined
- Mathematical operation on undefined variables would return NaN (not a number)
- Concatenating a string with an undefined variable would return an undefined string
- Naming convention camelCase for variable names
- The difference between var, let, and const variable declaration keywords
  - var is easily overridden
  - let: variable with the same name can only be declared once.
  - const: read-only variable, cannot be reassigned. (naming convention is all uppercase - immutable variables)
- Basic operations in Javascript: multiplication, addition, subtraction, and division.
- Increasing a variable by one with shorthand: i++ and i-- for the opposite.
- Decimal numbers are the ones that have float points or called float.
- The remainder operator %, the difference between the modulus operator is that it does not work with negative numbers.
- Everything on the right side of the assignment will be evaluated first.
- Operators such as +=; -=; \*=; /=
- Escaping literal quotes in a string by placing a backslash in front of the quote and escape sequence.
- Concatenation operator
- Using bracket notation to get a character at a specific index in a string.

# Day 2

![day-two-image](./images/dayTwo.png)

Today I have learned:

- Use bracket notation to get the value at a specific index in a string (`[]`) or entries in an array.
- The last letter of a string `const firstName = "Ada"` is `const lastLetter = firstName[firstName.length - 1]`, and the same principle applies for the nth last elements.
- Store multiple values in a variable called an Array.
- Multi-dimensional array is arrays nested in arrays.
- Using bracket notation to change the entry value of an array.
- Append data to the end of an array using `push()` method and `pop()` doing the opposite.
- `shift()` is used to remove the first element in the array and `unshift` is to remove the first element.
- Function is the reusable blocks of code that we divide our code used by invoking or being called with a function name followed by parentheses.
- Parameters are placeholders that are to be put into a function when it is called or invoked, and the actual values that are passed (put into) the parameters are called arguments.
- Return a value from a function with a return statement.
- Scope refers to the variable's visibility, which is where they can be seen and accessed in the code.
- Global scope vs local scope, and they could have the same name declaration.
- A function without a return statement would return an undefined value.
- A return value from a function can be stored in a variable.
- Queue data structure is when new items are added at the back of the queue and old items are taken off in front of the queue.
- Boolean data type.
- `if` statement is used to make decisions in code.
- Equality operator (`==`) which returns true OR false under certain circumstances with auto type conversion, is different from the assignment operator (`=`) as well as to compare with strict equality (`===`) with no auto type comparison and same with `!=` and `!==` in terms of auto data type conversion when comparing.
- `typeof` operator determines the data type of a variable.
- Greater than (`>`), greater than or equal (`>=`), less than (`<`), less than or equal (`<=`) operator has auto data type conversion.
- The logical and operator (`&&`) returns true if and only if the operands to the left and right of it are true.

# Day 3

![day-three-image](./images/dayThree.jpg)

Today I have learned:

- The (`||`) return true if either of the operands is true, otherwise it return false.
- `else` statement will be executed as an alternate block when if statement condition is false.
- Chain multiple `if` statement with `else if`.
- Logical order in `if else` statement is important since the function will be executed from the top.
- A `switch` statement compares values to `case` statements which define various possible value and `case` statement are tested with `(===)` and `default` statement as the last one in case no matching was found.
- Cases in `switch` statement can be combined when the have the same output.
- Short way to compare `(a === b)` without a `if` statement because the equality operator always return true or false.
- when the `return` statement is reached, the execution of a function stops and controls the return to the calling location.
- Javascript objects and access object data by using properties, numbers or strings can be used as properties.The number value properties will be typecasted as a string type.
- There are two way to access object property, by using `.` or `([])` which are called `Dot Notation` or `Bracket Notation`.
- Access the value of a propertiy in object by assign that property name to a variable and use it with object varible along with bracket notation.
- Adding a property in Javascript object has the same approach as accessing them and for deletion using `delete` keyword followed by the property value access.
- Using object as a key-value storage for tabular data instead of using `switch` or `if else` statement.

# Day 4

![day-four-image](./images/dayFour.jpg)

Today I have learned:

- Check if a property exist in an object with `.hasOwnProperty()` method which will return `true` or `false` depend on if the property exists in the object.
- Javascript object can be used to store flexiable and complicated data structure including the arbitrary combination of strings, numbers, booleans, arrays, functions, and objects.
- Accessing the sub-properties of an object, nested arrays by using the combination of dot and bracket notation.
- The `While` loop run until the specific condition is no longer valid.
- The `For` loop run the code specific multiple of times.
- The `do...while` loop makes sure the code in the loop gets executed at least one.
- Recursive function `(function multiplyAll(arr,n) == function multiplyAll(arr, n-1) * arr[n-1])` as an example intead of using `for` loop to calculate the multiplication for the first n elements in the array.
- The recursive function must have base case when they return to stop executing.

# Day 5

![day-five-image](./images/dayFive.jpg)

Today I have learned:

- `Math.random()` generate random decimal numbers from 0 (inclusive) and 1 (exclusive).
- All function calls will be resolved before the `return` statement.
- How to generate a random number using `Math.random()`

* Use Math.random() to generate random numbers
* Multiply by range (example: by 20 will generate 20 numbers)
* Use `Math.floor()` to round the decimal number to the nearest float point.
* The `Math.random()` method will never return a number 1 so it will never get to 20.

- How to generate a random number in a given range using `Math.random()`
  - `(Math.floor(Math.random() * (max - min + 1)) + min` will generate a random number that is greater than or equal to min and less than or equal to max.
- Using `parseInt()` method to convert a string to a number. If the first character of a string cannot be converted into a number it returns `NaN`.
- Using `parseInt()` method to convert a binary number to an integer with the second parameter called `radix` which represent the base of the number. `(example: parseInt('11', 2) return 3)`
- Using ternary (conditional) operator as an alternative method to `if...else` statement(example `(return a === b ? "Equal" : "Not Equal")`).
- Best practise to separate multiple conditional statement into lines in ternary operator.
- Use recursive function to backtrack constructing an array from 1 to the n parameter in

  ```javascript
  function countup(n) {
    if (n < 1) {
      return [];
    } else {
      const countArray = countup(n - 1);
      countArray.push(n);
      return countArray;
    }
  }
  ```

- This is an alternative way for using `for` loop, using `unshift()` method to do the other way around.

- Using recursive to backtrack constructing an array with a given range

  ```javascript
  function rangeOfNumbers(startNum, endNum) {
    if (endNum < startNum) {
      return [];
    } else {
      const arr = rangeOfNumbers(startNum, endNum - 1);
      arr.push(endNum);
      return arr;
    }
  }
  ```

# Day 6

![day-six-image](./images/daySix.jpg)

Today I have learned:

- ES6 or ECMAScript is the standardized version of Javascript.
- `let` keyword in ES6 can also be used only locally in a scope.
- Objects or arrays assigned with a `const` keyword are immutable which means, the whole unit itself cannot be changed but its element can.
- Use `Object.freeze` to avoid data from mutation.
- Use arrow function to write concise anonymous function, that is when an function is passed as an argument of another function and will not be reused.
- Arrow functions that do not have a body or only return a value can omit `return` keyword and the brackets surrounding.
- If the arrow function only has one parameter, the parentheses enclosing the parameter.
- ES6 introduced default parameters to the function, the default value will be used when no argument is passed into the function.
- Using rest parameter for function parameters.

# Day 7

![day-seven-image](./images/daySeven.jpg)

Today I have learned:

- Spread operator allow us to expand an array and other expressions where multiple elements or parameters are expected.
- Spread operator only works in-place like when in array literal or an argument to a function (example use case to copy an array).
- Destructuring assignment is a new feature introduced in ES6.
- Assign a new variable names when extract values using destructuring by adding column followed by a desired name in an object.
- Destructuring and change variales names from the nested objects.
- Destructuring an array and the use of comma to reach to the desired index.
- Using rest parameter with array destructuring

  ```javascript const [a, b, ...arr] = [1, 2, 3, 4, 5, 7];

  ```

- Cannot use the rest syntax to catch a subarray that leaves out the last element of the original array.
- Use rest element to emulate the behavior of `array.prototype.splice()`, the function below return a sub-array of the original array that omit the first 2 elements.

```javascript
function removeFirstTwo(list) {
  const [, , ...shortList] = list;
  return shortList;
}
```

- Use destructuring assignment to pass an object as a function's argument. This effectively destructure the object that sent to the function.

```javascript
const profileUpdate = (profileData) => {
  const { name, age, nationality, location } = profileData;
};

const profileUpdate = ({ name, age, nationality, location }) => {};
```

# Day 8

![day-seven-image](./images/dayEight.jpg)

Today I have learned:

- Tempalate literal enables us to create multi-line string or to use string interpolution to create string by using backticks.
- Using object property short-hand to write concise Object literal declaration.

```javascript
const getMousePosition = (x, y) => ({
  x: x,
  y: y,
});

`and`;

const getMousePosition = (x, y) => ({ x, y });
```

- When declaring a function for a property in an object, remove the function keyword and colon together.

# Day 9

![day-nine-image](./images/dayNine.jpeg)

Today I have learned:

- In ES6, a `class` declaration has a `constructor` method that is invoked using `this` keyword (explicitly) and if there is no `constructor` method is being defined then it takes no arguments.
- The constructor is invoked when there is a `new` keyword to create a new object.
- Uppercamel case is used to as naming convention for ES6 class name.
- The `constructor` is a special method to create and initilize object created with class.

```javascript
class Vegetable {
  constructor(name) {
    this.name = name;
  }
}
```

- Use getters and setters method to control the property of an object.
- Getter functions is used to get the value of the object's private values without having users accessing the private value of the variables.
- Setter functions is used to modify, override, calculate the value of the object private variables.

```javascript
class Thermostat {
  constructor(F) {
    this.F = F;
  }
  // get the temp in C
  get temperature() {
    return (5 / 9) * (this.F - 32);
  }
  set temperature(C) {
    return (this.F = (C * 9.0) / 5 + 32);
  }
}
```

- Create a `module` script to use ES6 features of `import` and `export`.
- There are 2 ways to export functions to share with other javascript file: one is use the `export` keyword directly in the function itself or use it in the export statement `(export {})`and the same approach to `import`.
- Use `import * as someThing from ""` to import all contents of a file to be used in another file and access them as properties of that alias of all content just created.
- Using `export default` to create a default fallback value for a module or a file and there is import statement `{}` for `export` default.
- Javascript promise using asynchronous function. A promise is a constructor function which is used by `new` keyword to create one.
- The Promise takes a function as an argument and 2 parametes of resolve and reject which are used to determine the outcome of the promise.

```javascript
const makeSeverRequest = new Promise((resolve, reject) => {});
```

# Day 10

![day-ten-image](./images/dayTen.jpeg)

Today I have learned:

- The `resolve` parameter is used to do something when the promise is a success and the other way aroud with the `reject` paraneter.If there is not parameter is used, the promise stuck in pending forever.
- The `promise` parameters take arguments to to process the data receieved.
- Use `then()` method is to handle fulfilled promise, executed immediately right after the promise is fulfilled with `resolve`.
- Use `catch()` method is used to handle the `reject` and the parameter of the inside callback function is passed to `reject` method.
- Regular express or `regex` is used to match parts of strings.
- Using `test()` method to determine the match in which it returns whether `true` or `false`.
- Regrex uses (/text/) to create a single expression to search the literal match in a string and use `alternation` `OR` operator `|`. example (`/textOne|textTwo|textThree`).
- Using flag `i` at the end of the regrex expression which is to ignore the case of the string.
- Use `match()` method with the regrex in parenthesis and apply it to a string to return the literal match aka extract it.
- The `g` flag helps to return the literal match more than once.
- Use `.` wildcard character to match any one letters.
- Use `[]` character class to combine both specifical match (`/text/`) and (`/text/.`) which is (`/b[aiu]/g`) that match ALL strings thah has `b` and `g` and targeting only the ones that has `aiu`.

# Day 11

![day-eleven-image](./images/dayEleven.jpg)

Today I have learned:

- Built-in feature in regrex that helps match multiple characters in the strings. Example : to match all literal that has lowercase letters from a - e(`[a-e]`).
- Using `-` also works with numbers to match with multiple numbers and both numbers and literals like `/[a-z0-9]/ig`.
- Create negated character set that we do not wanna match by just putting the caret `^` character right after the regrex expression. Example: `/[^a-z]/gi.` and use as many caret characters as needed to exclude the wanted literals.
- Use character `+` to find the match of a character that is at least one time repeated, if that letter appears consecutively, it will return a single match and multiple matches if they are not consecutive.
- Use the star `*` character to find the match if a character appears 0 or more times

# Day 12

![day-twelve-image](./images/dayTwelve.png)

Today I have learned:

- Greedy matching and lazy matching with examples of `/t[a-z]/*i` to match all patterns that starts with `t` and ends with `i` with characters in between and `/t[a-z]/*?i` is used just to match wherever the literal starts with `t` and ends `i`.
- Regex can be used to look for a number of matches and can be used to search for patterns in specific positions in a string.
- The caret `^` besides to exclude certain characters in the literals, it can still be used to search patterns at the beginning of the string. If the match is not at the beginning of a string it returns `false` and `true` otherwise.This character must be placed at the beginning of the regrex.
- The `$` helps to search the patterns at the end of the string.This regrex character must be placed at the end of the regrex.
- The closest character `/\w+/` is equivalent to the expression of `/[a-zA-Z0-9_]+/`. Use with `test()` method to return a `boolean` value and with `match()` method to return the numbers of matches example of `/\w/g`.
- A short character class `/d` is used to match all character digits which is equivalent to the class of `/[0-9]/`. and `/\D/g` for non-digit characters.
- A guidline to set usernames such as:

* Users can only be alphanumeric characters.
* The only numbers in username can only be at the end and cannot start with a number.
* Username can be lowercase and uppercase.
* Username can be 2 character length and a two-letter username can only use alphabet letters as characters.

```javascript
let userCheck = /^[a-z][a-z]+\d*$|^[a-z]\d\d+$/i;
```

- Class expression of `/s` to match with white space including: carriage return, tab, form feed and new line character.And `\S` for non-white space characters.
- Using quatity specifier `{}` to match with the certain range of patterns. Example `/a{3,5}h/` to match with letter `a` that appears more in the range of (3,5) in the literal `"ah"`.
- An expression with a question mark `?` means the previous character is optional. `/colou?r/` would match `color` and `colour`.
- Javascript patterns instruct the program to look ahead in the string to look for patterns along the way.
- There are 2 types of look-aheads: positive look-ahead will make sure the searched patterns are there but not actually match and the negative look-ahead will make sure the search patterns are not there.
- Example of a look-ahead that satisfy the passord requirement which contains more than 5 chatacters and at least 2 consecutive digits `/(?=\w{6})(?=\w*\d{2})/`.
- Check for mixed grouping of characters using `/P(engu|umpk)in/g` which will potentially match `Penguin` and `Pumpkin`.
- Using `/(/w+)/` to match with capture group of words that repeat multiple times. A captured group of a string will be saved in a temporary variable one-indexed and accessed by `/` or '$' within the capture groups.
- Using `replace(regex, somethingToReplace)` to search for the match in the first parameter and second parameter is to replace.
- Using regular expression with `replace()` method to trim the white space at the beginning or at the end of the string

```javascript
let hello = "   Hello, World!  ";
let wsRegex = /^\s+|\s+$/g;
let result = hello.replace(wsRegex, "");
```

# Day 13

![day-thirtteen-image](./images/dayThirteen.jpg)

Today I have learned:

- The use of devTool in browser such as: Firefox and Chrome with `console.log()` as a debugging tool.
- It is the good practise to be aware of the value type before cheking what it is and having check points to see the status of calculations throughout the code helps narrow down where the problem is.
- Use `console.clear()` to clear all the logs from the console.
- Use `typeof` to check the data type, it is interesting to note that, `[]` is type object.
- Misspelled variable and function names can make the browser look for a non-existent object and complain in the form of reference error.
- Opening parentheses, brackets, curly braces, and quotes have a closing pairs is another form of syntax error that Javascript will complain.
- Take extra care when nesting code blocks or adding a callback function as an argument for a function.
- Making sure the consistency of using double quote and single quote, a `/` can be used to escape character.
- `Branch programs` is the one that do different things when certain conditions are met using `if , else if` statements. This process makes sure the program runs on the right branch.
- Sometimes, the funnction call that takes no argument is saved in the variable for later use.
- Make sure the passing arguments for a function in a correct order since different data types can result in runtime error and same data type will not make any sense with the logic.
- Off by one error(OBOE) is when an array or a string is manipulated such as (`slice, accessing a certain index or looping through the indices`).The OBOE indicates the error when accessing the index that is equal to the length of the array or missing indexes when looping through its indices.
- Use Caution When Reinitializing Variables Inside a Loop, particularly when a variable value needs re-initialization or resetting variable in a loop would cause the infinite loop.
- There is a dreaded infinite loop that has no terminal condition to break the loop which causes the program mayhem, freeze and crash the browser.

# Day 14

![day-fourteen-image](/images/dayFourteen.jpg)

Today I have learned:

- One dimensional array that does not have any nested arrays could include valid javascript data types.
- Multi-dimensial array includes other arrays that can store complex data types such as object.
- Using bracket notation to access && assign values to the value of array indexes `[]`.
- Arrays are mutable, `push()` and `unshift()` method add items to the end and the beginning of the array respectively.
- Method `pop()` and `shift()` function opposite to `push()` anf `unshift()` respectively.
- Using `splice()` method with the first argument to which item to begin remove and the second argument is the number of items to remove.
- The third argument in `splice()` method adds one or more elememts to the array after removing certain elements at the removing indexes.
- The `slice()` method extract elements from the origional array without modifying it, it takes 2 arguments, the first one is from the index it begins with up to (not including the item at the second arguemnt index).
- Another way of copying an array is to use `spread (...)` syntax.
- Using spread operator can help combine arrays or inserting one array to another

```javascript
let thisArray = ["sage", "rosemary", "parsley", "thyme"];

let thatArray = ["basil", "cilantro", ...thisArray, "coriander"];
```

- Method `indexOf()` takes one argument as a parameter and return the index of of that parameter in the array, it returns `-1` when the item does not exist on the array.
- Javascript offer built-in method such as `forEach()`, `every()`, `map` etc to iterate through the items in the array based on data items meet a certain set of criteria but using `for loop` statement give us the most control and flexibility.
- Array can contain nested arrays which can become complex data structures with different levels of depth, the outer-most array is level one.
- Key-value pair in Javascript, basicallym they are pieces of data(value) that is mapped to the identifier as keys.
- Objects can be also nested in another objects just like array in Javascript.
- Using bracket notation is very useful when we wanna access the property of an object in a dynamic way in case the value of the property is not known before runtime.
- Use `for...in` statement to loop through the object keys in an object.
- Use `Object.keys()` that takes an argument as an object and return an array of that object properties.

# Day 15

![day-fifteen-image](./images/dayFifteen.jpg)

Today I have learned:

- Convert from Celsius to Fa : F = C \* 9/5 + 32.
- Reverse a string by `reverse()` method.
- Factorize a number using `for...loop`.

```javascript
function factorialize(num) {
  if ((num === 0) | (num === 1)) {
    return 1;
  }
  for (let i = num - 1; i >= 1; i--) {
    num *= i;
  }
  return num;
}
```

- Find a length of the longest word in a sentence

````javascript
function findLongestWordLength(str) {
  //look for a longest word
  let allWords = str.split(' ')
  // set a milestone to compare as iterating through the array
  let maxLength = 0
  for(let i =0; i < allWords.length; i++){
    if(allWords[i].length > maxLength){
      maxLength = allWords[i].length
    }
  }
  return maxLength;
}```
- `Or`

```javasript
function findLongestWordLength(s) {
  return s
    .split(' ')
    .reduce((longest, word) => Math.max(longest, word.length), 0);
}
````

# Day 16

![day-sixteenth-image](./images/daySixteenth.jpg)

Today I have learned:

- Problem 1: return an array of large numbers of for each of the sub-array in the array

```javascript
function largestOfFour(arr) {
  let newArr = [];
  for (let i = 0; i < arr.length; i++) {
    let largeNumber = arr[i][0];
    for (let j = 1; j < arr[i].length; j++) {
      if (arr[i][j] > largeNumber) {
        largeNumber = arr[i][j];
      }
    }
    newArr[i] = largeNumber;
  }
  return newArr;
}
```

- Problem 2: Check of the string ends with a given string

```javascript
function confirmEnding(str, target) {
  return str.slice(str.length - target.length) === target;
}
```

- Problem 3: Repeat a string for a number of times

```javascript
function repeatStringNumTimes(str, num) {
  let newString = "";
  if (num < 0) {
    return "";
  } else {
    for (let i = 0; i < num; i++) {
      newString += str;
    }
  }
  return newString;
}
```

- Problem 4: Return a truncated string if its length exceeds the given number

```javascript
function truncateString(str, num) {
  if (str.length > num) {
    return str.slice(0, num) + "...";
  } else {
    return str;
  }
}
```

- Problem 5: Return the first element of the array that satisfy the condition of another function.

```javascript
function findElement(arr, func) {
  return arr.find((item) => (func(item) ? item : undefined));
}
```

- Problem 6: Check if a value is classified as a boolean primitive

```javascript
function booWho(bool) {
  return typeof bool === "boolean";
}
```

# Day 17

![day-seventeenth-image](./images/daySeventeenth.jpg)

Today I have learned:

- Problem 7: Capitialize the first letter of each word in a string

```javascript
function titleCase(str) {
  let strArr = str.split(" ");
  for (let i = 0; i < strArr.length; i++) {
    strArr[i] = strArr[i][0].toUpperCase() + strArr[i].slice(1).toLowerCase();
    if (strArr[i].toLowerCase() === "the" || strArr[i].toLowerCase() === "of") {
      strArr[i] = strArr[i].toUpperCase();
    }
  }
  return strArr.join("");
}
```

- Problem 8: Insert an array at a specific index of another array

```javascript
function frankenSplice(arr1, arr2, n) {
  return arr2.slice(0, n).concat(arr1, arr2.slice(n));
}
```

- Problem 9: Remove all falsy values from the array with mutating the original one

```javascript
function bouncer(arr) {
  const newArray = [];
  for (let i = 0; i < arr.length; i++) {
    if (arr[i]) {
      newArray.push(arr[i]);
    }
  }
  return newArray;
}
```

- Problem 10: Return the lowest index of an array where a given number is inserted

```javascript
function getIndexToIns(arr, num) {
  let sortedArr = arr.sort();
  let lowestIndex = 0;
  for (let i = 0; i < sortedArr.length; i++) {
    if (sortedArr[i] < num) {
      lowestIndex += 1;
    }
  }
  return lowestIndex;
}
```

- Problem 11: check if the second element of the array contains all the letters of the first item

```javascript
function mutation(arr) {
  const firstElem = arr[0].toLowerCase();
  const secondElem = arr[1].toLowerCase();
  for (let i = 0; i < secondElem.length; i++) {
    if (firstElem.indexOf(secondElem[i]) < 0) return false;
  }
  return true;
}
```

- Problem 10: Split an array to sub-arrays with a size of a given number

```javascript
function chunkArrayInGroups(arr, size) {
  let newArray = [];
  for (let i = 0; i < arr.length; i += size) {
    newArray.push(arr.slice(i, i + size));
  }
  return newArray;
}
```

# Day 18

![day-eighteenth-image](./images/dayeighteenth.jpg)

Today I have learned:

_Object Oriented Programming_

- Object in Javascript used to model the real-world objects.
- Create an object in Javascript.
- If a variable name of an object varies, then references to that name needs to be updated as well, however, using `this` keyword to access the object properties makes the object reusable without the need of updating the references.
- Constructors behave like the blueprint which are used to create an object.
- Constructors conventions:
  1.Capitalized name.
  2.Using `this` keyword to create properties of an object.
- Example:

```javascript
function Bird() {
  this.name = "Albert";
  this.color = "blue";
  this.numLegs = 2;
}
// make another instance of Bird object with new operator
const secondBird = new Bird();
```

- Passing argument for the constructor for it to be reusable

```javascript
function Bird(name, color) {
  this.name = name; // own properties
  this.color = color;
}

Bird.prototype.numLegs = 4; // prototype properties.

const secondBird = new Bird("Pui", "gray");

secondBird instanceof Bird;
```

- Use `instanceof` operator to verify of an object is an instance of a constructor
- Use `prototype` so that the properies are shared among all instances.
- The properties in the object that are created with the constructor are called `own properties` and the other type is called `prototype`.
- The use `constructor` property for helping verify the object of the constructor function object. `constructor` refers to the constructor function that creates the object.
- `prototype` can be written in form of object

```javascript
function Dog(name) {
  this.name = name;
}

Dog.prototype = {
  constructor: Dog, // manually define the constructor
  numLegs: 4,
  eat: function () {},
  describe: function () {},
};

const Bull = new Dog();
```

- An object that inherits the prototype of the constructor that created it and proved by `Dog.prototype.isPrototypeof(Bull)`
- Every object in Javascript has `prototype`, a `prototype` itself is an object and its prototype is `Object.prototype` which is the supertype of all objects.
- The principle in programming is called `DRY` which is to not repeat yourself, so that there will be less errors and less work for programmers by using techunique `inheritance`
- There is an alternative approach to `new` operator to create an instance for an constructor object which is `Object.create(obj)`, by replacing `obj` by the constructor object prototype, the new object inherits the protype of the constructor object.
- Make substype to inherit from the supertype object :

```javascript
Dog.prototype = Object.create(Animal.prototype); // Animal is the supertype that has a method that is shared with the Dog instance now.
```

- Keep in mind to manually modify the constructor of the object prototype inheritance constructor `Dog.prototype.constructor = Dog` not animal.

# Day 19

![day-nineteenth-image](./images/dayNineteenth.jpg)

Today I have learned:

- Besides of getting the object prototype inheritance from a supertype, the object constructor can have its own unique methods.
- The formula for children to inherit methods from its parents object:

```javascript
ChildObject.prototype = Object.create(ParentObject.prototype);
```

- When inherits from the supertype, using `child.prototype.method` to assign it with anoher value to override the inheritance value.
- Using `mixins` to share methods between unrelated objects instead of inheritance, the conventtion name is camel case for `mixins`.

```javascript
let bird = {
  name: "Donald",
  numLegs: 2,
};

let boat = {
  name: "Warrior",
  type: "race-boat",
};

let glideMixin = function (obj) {
  obj.glide = function () {
    console.log("sharing using mixins");
  };
};
glideMixin(bird);
glideMixin(boat);
```

- In Javascript, a function always has access to the context in which it was created.
- A private property in an object can only access by its contructor object method, not any part of the codebase.

```javascript
function Bird() {
  let weight = 15; // weight is a private variable that can only be accessed with getWeight method.
  this.getWeight = function () {
    return weight;
  };
}
```

- The function with no name and wrapped by a pair of `()` and an empty `()` with no arguments is the immediately invoked function express

```javascript
(function () {
  console.log("A cozy nest is ready");
})();
```

- The immediately invoke function express can be used to create a module that can be accessed anywhere in the code base by combining all the mixins as properties of an object of the IIFE return statement.

```javascript
let isCuteMixin = function (obj) {
  obj.isCute = function () {
    return true;
  };
};
let singMixin = function (obj) {
  obj.sing = function () {
    console.log("Singing to an awesome tune");
  };
};

let funModule = (function () {
  return {
    isCuteMixin: function (obj) {
      obj.isCute = function () {
        return true;
      };
    },
    singMixin: function (obj) {
      obj.sing = function () {
        console.log("Sing to an awesome tune");
      };
    },
  };
})();
```

# Day 20

![day-tweetith-image](./images/dayTweentith.jpg)

_Functional Programming_

Today I have learned:

- Functional programming is the programming style that is independent, same input results the same output and functions regardless of any other factors which are called: `Isolated function` - `Pure function ` which does not cause the side effect for the outcome.
- `callbacks` functions are the ones that are passed into or slipped into to decide the invocation of a function and alse called `lambda` and are called first class functions.
- Functions that takes other functions as parameters are called `higher order` functions.
- Be cautious when using `splice()` since the method modifies the array.
- The core principle in functional programming is the function does not change things for better bug prevention.It should not mutate the original variables.
- The other principle is that of the function depends on an object or a variable present then pass that in as the function argument so that the function is easier to test and will not depend on anything in your program.
- Example of functional programming: Dont alter a variable or an object, intead copy it and so something with it.

```javascript
// The global variable
const bookList = [
  "The Hound of the Baskervilles",
  "On The Electrodynamics of Moving Bodies",
  "Philosophiæ Naturalis Principia Mathematica",
  "Disquisitiones Arithmeticae",
];

// Change code below this line
function add(arr, bookName) {
  let newArray = [...arr];
  newArray.push(bookName);
  return newArray;

  // Change code above this line
}

// Change code below this line
function remove(arr, bookName) {
  let newArray = [...arr];
  const book_index = newArray.indexOf(bookName);
  if (book_index >= 0) {
    newArray.splice(book_index, 1);
    return newArray;

    // Change code above this line
  }
}
```

- The use of `array.prototype.map` objec or simple `map(item, index, originalArray)` that iterate through the array without mutating the original array.This is considered a `pure` function.
- The use of `forEach()` and `for loop` are also recommended as alternatives as `map()`

# Day 21

![day-tweentyfirst](./images/dayTweentyfirst.jpg)

Today I have learned:

- The use of `Array.prototype.filter` that filter the elements in the array based on the callback functions, it does not mutate the
- The combonation of using `filter()` and `map()` together to sort an array of objects.
- Using `for loop` statement and `forEach()` are recommended methods instead of `filter()`.
- The `slice()` method is used to make a copy of an array without mutating it.
- Concatenation means to join which works well with a string or an array with `concat()` method.Concatenation is one way of functional programming which does not mutate the original array but to merge them together and return a new array.
- The use of `reduce()` is general for all javascript array operations which can potentially cover `map()` and `filter()`.
- `parseInt()` and `parseFloat()`
- Javascript bult-in `sort()` method applied on Unicode value points can sometimes output unexpectedly, therefore, a callback function is included to prevent this issue.
- The `split()` methods works on string since its immutable.One thing to remember when splitting is to `trim()` the whitespace of the string and split with one or more white space using `/\S+/` regrex for expected behaviour.
- The `join()` method is used to join the array together to make a string.
- The `every()` method is used to determine if every item of the array passed a particular test of its callback function.
- The `some()` method is used to determine if any item in the array passed a particular test of its callback function.
- Term `arity` of a function means number of arguments in a function and `currying function` means to restructor the function to take the `arity` of 1 and return another function inside it and so on.

# Day 22

![day-twentyseond](./images/dayTwentysecond.jpg)

Today I have learned:

- Using `for loop` statement and `sort()` combination to calculate the sum between 2 given numbers in an array, the smallest number never comes first.
- `Arithmetic progression summing` formula: ((startNum + endNum) \* numCount) / 2.
- Return the symmetric difference of 2 arrays.
- Index of `-1` means the item does not exist in the array.
- To call another function within a function whose function takes parameters as arguments as placeholder for the outer function.
- Review `rest` parameter allows function to take unlimited arguments and put them in an array.
- The `object.value()` return an array of that object values and the `argument` object that contain all argument for the object in the form of array-like object.
- Comparing a key-value pair with an object to find a match using `for loop` and `if` statement.
- Regrex `/\s|_|(?=[A-Z])/` to encounter whitespace, underscore, and followed by the uppercase letters.
- The use of `charAt()` to interact with indexes in a string.
- One thing to note when searching and replacing an item in an array is that it is a good tip to find the to-be-replace item index and then manipulate it if there is such conditions before replace it with another value.
- One thing to note when returning a 2-D array from a given string, remember to return the accumulated array for each iteration to make sure the array is updated to contains sub-arrays.

```javascript
function pairElement(str) {
  const basePairs = {
    A: "T",
    T: "A",
    C: "G",
    G: "C",
  };
  let twoDArr = str.split("").reduce((array, block) => {
    if (basePairs.hasOwnProperty(block)) {
      array.push([block, basePairs[block]]);
      return array;
    }
  }, []);
  return twoDArr;
}

console.log(pairElement("GCG"));
```
