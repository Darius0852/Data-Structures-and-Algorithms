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
## Compound Assignment with Augmented Addition

In programming, it is common to use assignments to modify the contents of a variable. Remember that everything to the right of the equals sign is evaluated first, so we can say:
```
myVar = myVar + 5;
```
to add 5 to myVar. Since this is such a common pattern, there are operators which do both a mathematical operation and assignment in one step.

One such operator is the += operator.
```
var myVar = 1;
myVar += 5;
console.log(myVar);
```
6 would be displayed in the console.

Convert the assignments for a, b, and c to use the += operator.

```
var a = 3;
var b = 17;
var c = 12;

// Only change code below this line
a += 12;
b += 9;
c += 7;
```

## Compound Assignment With Augmented Subtraction

Convert the assignments for a, b, and c to use the -= operator.

```
var a = 11;
var b = 9;
var c = 3;

// Only change code below this line
a -= 6;
b -= 15;
c -= 1;
```

## Compound Assignment With Augmented Multiplication

Convert the assignments for a, b, and c to use the *= operator.

```
var a = 5;
var b = 12;
var c = 4.6;

// Only change code below this line
a *= 5;
b *= 3;
c *= 10;
```

## Compound Assignment With Augmented Division

Convert the assignments for a, b, and c to use the /= operator.

```
var a = 48;
var b = 108;
var c = 33;

// Only change code below this line
a /= 12;
b /= 4;
c /= 11;
```

## Declare String Variables

Create two new string variables: myFirstName and myLastName and assign them the values of your first and last name, respectively.

```
var myFirstName = "Darius";
var myLastName = "Ghomashchian";
```

## Escaping Literal Quotes in Strings

When you are defining a string you must start and end with a single or double quote. What happens when you need a literal quote: " or ' inside of your string?

In JavaScript, you can escape a quote from considering it as an end of string quote by placing a backslash (\) in front of the quote.
```
var sampleStr = "Alan said, \"Peter is learning JavaScript\".";
```
This signals to JavaScript that the following quote is not the end of the string, but should instead appear inside the string. So if you were to print this to the console, you would get:
```
Alan said, "Peter is learning JavaScript".
```

Use backslashes to assign a string to the myStr variable so that if you were to print it to the console, you would see:
```
I am a "double quoted" string inside "double quotes".
```

```
var myStr = "I am a \"double quoted\" string inside \"double quotes\".";
console.log(myStr);
```

## Quoting Strings with Single Quotes


Remember, a string has the same kind of quote at the beginning and end. But if you have that same quote somewhere in the middle, the string will stop early and throw an error.
```
goodStr = 'Jake asks Finn, "Hey, let\'s go on an adventure?"'; 
badStr = 'Finn responds, "Let's go!"';
```
Here badStr will throw an error.

Below is another example (answer):
```
var myStr = '<a href="http://www.example.com" target="_blank">Link</a>';
```

## Escape Sequences in Strings

Quotes are not the only characters that can be escaped inside a string. There are two reasons to use escaping characters:

1. To allow you to use characters you may not otherwise be able to type out, such as a carriage return.
2. To allow you to represent multiple quotes in a string without JavaScript misinterpreting what you mean.
   We learned this in the previous challenge.

| Code |      Output     |
|:----:|:---------------:|
|  \'  |   single quote  |
|  \"  |   double quote  |
|  \\  |    backslash    |
|  \n  |     newline     |
|  \r  | carriage return |
|  \t  |       tab       |
|  \b  |  word boundary  |
|  \f  |    form feed    |

Note that the backslash itself must be escaped in order to display as a backslash.

Example - To generate this:
```
FirstLine
    \SecondLine
ThirdLine
```
We use this:
```
var myStr = "FirstLine\n\t\\SecondLine\nThirdLine"; 
```
## Concatenating Strings with Plus Operator

In JavaScript, when the + operator is used with a String value, it is called the *concatenation* operator. You can build a new string out of other strings by concatenating them together.

Example;
```
'My name is Alan,' + ' I concatenate.'
```

**Note**: Watch out for spaces. Concatenating does not add spaces between concatenated strings, so you'll need to ass them yourself. 

Example:
```
var ourStr = "I come first. " + "I come second.";
```
The string:
I come first. I come second.
would be displayed in the console.

## Concatenting Strings with the Pluc Equals Operator

We can also use the += operator to concatenate a string onto the end of an existing string variable. This can be very helpful to break a long string over several lines.

Example:

```
var myStr = "This is the first sentence. ";
myStr += "This is the second sentence.";
```

## Constructing Strings with Variables

Sometimes you will need to build a string, Mad Libs style. By using the concatenation operator (+), you can insert one or more variables into a string you're building.
```
var myName = "Darius";
var myStr = "Hello my name is " + myName + ", nice to meet you";
```

## Appending Variables to Strings

Just as we can build a string over multiple lines out of string literals, we can also append variables to a string using the plus equals (+=) operator.

```
var someAdjective = "fun";
var myStr = "Learning to code is ";
myStr += someAdjective;
```

## Find the Length of a String

You can find the length of a String value by writing .length after the string variable or string literal.

```
// Setup
var lastNameLength = 0;
var lastName = "Lovelace";

// Only change code below this line

lastNameLength = lastName.length;
```

## Use Bracket Notation to Find the First Character in a String

Bracket notation is a way to get a character at a specific index within a string.

Most modern programming languages, like JavaScript, don't start counting at 1 like humans do. They start at 0. This is referred to as Zero-based indexing.

For example, the character at index 0 in the word Charles is C. So if var firstName = "Charles", you can get the value of the first letter of the string by using firstName[0].
firstLetter would have a value of the string C.

Example: 
```
var firstName = "Charles";
var firstLetter = firstName[0];
```

## Understand String Immutability

In JavaScript, String values are immutable, which means that they cannot be altered once created.

Example: 
```
var myStr = "Bob";
myStr[0] = "J";
```
cannot change the value of myStr to Job, because the contents of myStr cannot be altered. Note that this does not mean that myStr cannot be changed, just that the individual characters of a string literal cannot be changed. The only way to change myStr would be to assign it with a new string, like this:
```
var myStr = "Bob";
myStr = "Job";
```

## Use Bracket Notation to Find the Nth Character in a String

You can also use bracket notation to get the character at other positions within a string.

Remember that computers start counting at 0, so the first character is actually the zeroth character.

Example:
```
var firstName = "Ada";
var secondLetterOfFirstName = firstName[1];
```
secondLetterOfFirstName would have a value of the string d.

## Use Bracket Notation to Find the Last Character in a String

In order to get the last letter of a string, you can subtract one from the string's length.

For example, if var firstName = "Charles", you can get the value of the last letter of the string by using firstName[firstName.length - 1].

Example:
```
var firstName = "Charles";
var lastLetter = firstName[firstName.length - 1];
```
lastLetter would have a value of the string s.

## Use the Brakcet Notation to Find the Nth-to-Lats Character in a String

You can use the same principle we just used to retrieve the last character in a string to retrieve the Nth-to-last character.

For example, you can get the value of the third-to-last letter of the var firstName = "Charles" string by using firstName[firstName.length - 3]

Example:
```
var firstName = "Charles";
var thirdToLastLetter = firstName[firstName.length - 3];
```
thirdToLastLetter would have a value of the string l.






















