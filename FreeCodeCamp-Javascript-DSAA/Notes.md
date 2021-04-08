# Notes

## Basics

JavaScript provides eight different data types which are undefined, null, boolean, string, symbol, bigint, number, and object.
Variables allow computers to store and manipulate data in a dynamic fashion. They do this by using a "label" to point to the 
data rather than using the data itself. Any of the eight data types may be stored in a variable.

We tell JavaScript to create or declare a variable by putting the keyword var in front of it, like so:
```
var ourName;
```
creates a variable called ourName. In JavaScript we end statements with semicolons. Variable names can be made 
up of numbers, letters, and $ or _, but may not contain spaces or start with a number.

In JavaScript, you can store a value in a variable with the assignment operator (=).
```
myVariable = 5;
This assigns the Number value 5 to myVariable.
```
If there are any calculations to the right of the = operator, those are performed before the value is assigned to the variable on the left of the operator.

After a value is assigned to a variable using the assignment operator, you can assign the value of that variable to another variable using the assignment operator.
```
var myVar;
myVar = 5;
var myNum;
myNum = myVar;
```
The above declares a myVar variable with no value, then assigns it the value 5. Next, a variable named myNum is declared with no value. Then, the contents of myVar (which is 5) is assigned to the variable myNum. Now, myNum also has the value of 5.

It is common to initialize a variable to an initial value in the same line as it is declared.
```
var myVar = 0;
```
Creates a new variable called myVar and assigns it an initial value of 0.

## Understanding Uninitialized Variables

When JavaScript variables are declared, they have an initial value of undefined. If you do a mathematical operation on an undefined variable your result will be NaN which means "Not a Number". If you concatenate a string with an undefined variable, you will get a literal string of undefined.

## Understanding Case Sensitivity in Variables

In JavaScript all variables and function names are case sensitive. This means that capitalization matters.

MYVAR is not the same as MyVar nor myvar. It is possible to have multiple distinct variables with the same name but different casing. It is strongly recommended that for the sake of clarity, you do not use this language feature.

### Best Practice

Write variable names in JavaScript in camelCase. In camelCase, multi-word variable names have the first word in lowercase and the first letter of each subsequent word is capitalized.

### Examples
```
var someVariable;
var anotherVariableName;
var thisVariableNameIsSoLong;
```
## Add Two Numbers with JavaScript

Number is a data type in JavaScript which represents numeric data.

Now let's try to add two numbers using JavaScript.

JavaScript uses the + symbol as an addition operator when placed between two numbers.

Example:
```
myVar = 5 + 10;
```
myVar now has the value 15.

## Subtract One Number from Another with JavaScript

We can also subtract one number from another.

JavaScript uses the - symbol for subtraction.

Example
```
myVar = 12 - 6;
```
myVar would have the value 6.

## Multiply Two Numbers with JavaScript

We can also multiply one number by another.

JavaScript uses the * symbol for multiplication of two numbers.

Example
```
myVar = 13 * 13;
```
myVar would have the value 169.

## Divide One Number by Another with JavaScript

We can also divide one number by another.

JavaScript uses the / symbol for division.

Example
```
myVar = 16 / 2;
```
myVar now has the value 8.

## Increment a Number with JavaScript

You can easily increment or add one to a variable with the ++ operator.
```
i++;
```
is the equivalent of
```
i = i + 1;
```
Note: The entire line becomes i++;, eliminating the need for the equal sign.

## Decrement a Number with JavaScript

You can easily decrement or decrease a variable by one with the -- operator.
```
i--;
```
is the equivalent of
```
i = i - 1;
```
Note: The entire line becomes i--;, eliminating the need for the equal sign.

## Create Decimal Numbers with JavaScript

We can store decimal numbers in variables too. Decimal numbers are sometimes referred to as floating point numbers or floats.
e.g.
```
var ourDecimal = 5.7;
```

## Multiply Two Decimals with JavaScript

In JavaScript, you can also perform calculations with decimal numbers, just like whole numbers.
e.g.
```
var product = 2.0 * 2.5;
```

Note: Not all real numbers can accurately be represented in floating point. This can lead to rounding errors.

## Divide One Decimal by Another in JavaScript
```
var quotient = 4.4/2.0;
```

## Finding a remainder in JavaScript

The remainder operator % gives the remainder of the division of two numbers.
### Example
```
5 % 2 = 1 because
Math.floor(5 / 2) = 2 (Quotient)
2 * 2 = 4
5 - 4 = 1 (Remainder)
```
### Usage
In mathematics, a number can be checked to be even or odd by checking the remainder of the division of the number 2.
```
17 % 2 = 1 (17 is Odd)
48 % 2 = 0 (48 is Even)
```
## Javascript Linked Lists
