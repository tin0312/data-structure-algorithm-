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
- Operators such as +=; -=; *=; /=
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
- Recursive function `(function multiplyAll(arr,n) == function multiplyAll(arr, n-1) * arr[n-1])` as an example intead of using `for` loop  to calculate the multiplication for the first n elements in the array.
- The recursive function must have base case when they return to stop executing.


# Day 5

![day-five-image](./images/dayFive.jpg)

Today I have learned:

- `Math.random()` generate random decimal numbers from 0 (inclusive) and 1 (exclusive).
- All function calls will be resolved before the `return` statement.
- How to generate a random number using `Math.random()`
 + Use Math.random() to generate random numbers
 + Multiply by range (example: by 20 will generate 20 numbers)
 + Use `Math.floor()` to round the decimal number to the nearest float point.
 + The `Math.random()` method will never return a number 1 so it will never get to 20.
- How to generate a random number in a given range using `Math.random()`
  + `(Math.floor(Math.random() * (max - min + 1)) + min` will generate a random number that is greater than or equal to min and less than or equal to max.
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


- This is an alternative way for using `for` loop, using `unshift()` method to do the other way around.

- Using recursive to backtrack constructing an array with a given range

  ```javascript
  function rangeOfNumbers(startNum, endNum) {
  if (endNum < startNum) {
    return []
  } else {
      const arr = rangeOfNumbers(startNum, endNum - 1)
      arr.push(endNum);
      return arr
  }
}

# Day 6

![day-six-image](./images/daySix.jpg)

Today I have learned:

- ES6 or ECMAScript is the standardized version of Javascript.
- `let` keyword in ES6 can also be used only locally in a scope.
-  Objects or arrays assigned with a `const` keyword are immutable which means, the whole unit itself cannot be changed but its element can.
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
-  Cannot use the rest syntax to catch a subarray that leaves out the last element of the original array.
- Use rest element to emulate the behavior of `array.prototype.splice()`, the function below return a sub-array of the original array that omit the first 2 elements.

```javascript

function removeFirstTwo(list) {
  const [,, ...shortList] = list
  return shortList;
}
```

- Use destructuring assignment to pass an object as a function's argument. This effectively destructure the object that sent to the function.

```javascript
const profileUpdate = (profileData) => {
  const { name, age, nationality, location } = profileData;

}

const profileUpdate = ({name, age, nationality, location}) => {}
```

![day-seven-image](./images/dayEight.jpg)

Today I have learned: 

- Tempalate literal enables us to create multi-line string or to use string interpolution to create string by using backticks.
- Using object property short-hand to write concise Object literal declaration.

```javascript 

const getMousePosition = (x, y) => ({
  x: x,
  y: y
});

`and`

const getMousePosition = (x, y) => ({ x, y });

```

- When declaring a function for a property in an object, remove the function keyword and colon together.
