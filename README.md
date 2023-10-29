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