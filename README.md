# JavaScript-Algorithms
JS Documentations



              ============= JavaScript Fundamentals =================

JavaScript was invented by Brendan Eich in 1995, and became an ECMA standard in 1997.
ECMA-262 is the official name of the standard. ECMAScript is the official name of the language.

JavaScript is one of the 3 languages all web developers must learn:

   1. HTML to define the content of web pages

   2. CSS to specify the layout of web pages

   3. JavaScript to program the behavior of web pages

* Web pages are not the only place where JavaScript is used. 
* Many desktop and server programs use JavaScript.
* Node.js is the best known. Some databases, like MongoDB and CouchDB, also use JavaScript as their programming language.

Statments:

A computer program is a list of "instructions" to be "executed" by a computer.

In a programming language, these programming instructions are called statements.

A JavaScript program is a list of programming statements.

--------------------------------------------------------------------------------------------------------.
JavaScript Display Possibilities

Writing into an HTML element, using innerHTML. document.getElementById("demo").innerHTML = 5 + 6;
Writing into the HTML output using document.write().
Writing into an alert box, using window.alert().
Writing into the browser console, using console.log().

JavaScript Code Blocks

JavaScript statements can be grouped together in code blocks, inside curly brackets {...}.
The purpose of code blocks is to define statements to be executed together.
One place you will find statements grouped together in blocks, is in JavaScript functions:
-------------------------------------------------------------------------------------------------------.

Syntax:

 JavaScript syntax defines two types of values: Fixed values and variable values.
 Fixed values are called literals. Variable values are called variables.
 Numbers are written with or without decimals: 10.50 - 1001
 
Variables:

In a programming language, variables are used to store data values.
All JavaScript variables must be identified with unique names.

These unique names are called identifiers.

Identifiers can be short names (like x and y) or more descriptive names (age, sum, totalVolume).

The general rules for constructing names for variables (unique identifiers) are:

Names can contain letters, digits, underscores, and dollar signs.
Names must begin with a letter
Names can also begin with $ and _ (but we will not use it in this tutorial)
Names are case sensitive (y and Y are different variables)
Reserved words (like JavaScript keywords) cannot be used as names

------------------------------------------------------------------------------------------

Operators:

*Assignment operator (=) assigns a value to a variable.
  Assignment operators assign values to JavaScript variables.

Operator	Example	Same As
=	x = y	x = y
+=	x += y	x = x + y
-=	x -= y	x = x - y
*=	x *= y	x = x * y
/=	x /= y	x = x / y
%=	x %= y	x = x % y
**=	x **= y	x = x ** y

********************************************************.

*Arithmetic Operators
  Arithmetic operators are used to perform arithmetic on numbers:

Operator	Description
+	Addition
-	Subtraction
*	Multiplication
**	Exponentiation (ES2016)
/	Division
%	Modulus (Division Remainder)
++	Increment
--	Decrement

********************************************************.

*Comparison Operators
 Comparison and Logical operators are used to test for true or false.

Operator	Description
==	equal to
===	equal value and equal type
!=	not equal
!==	not equal value or not equal type
>	greater than
<	less than
>=	greater than or equal to
<=	less than or equal to
?	ternary operator

********************************************************.

*Logical Operators
 Logical operators are used to determine the logic between variables or values.

Operator	Description
&&	logical and
||	logical or
!	logical not

*******************************************************.

// TRUE 1
// FALSE 0
// && AND operator (multiply * )
// || OR operator (SUM +)
/*
true && true = true
true && false = false
false && true = false
false && false = false
====================
1 * 1 = 1 true
1 * 0 = 0 false
*/

/*
true || true = true
true || false = true 
false || true = true
false || false = false
=================
1 + 1 = 2 true
1 + 0 = 1 true
0 + 1 = 1 true
0 + 0 = 0 false
*/

/* 
var x = 10;
var y = 30;
var z = 50;
//Case 1
(x + y >= z || x > z/2)
//50 >= 50 || 10 > 25
// true || false
// true

//Case 1
(x + y >= z && x > z/2)
//50 >= 50 && 10 > 25
// true && false
// false
*/

=================================================================

JavaScript Data Types:

JavaScript variables can hold many data types: numbers, strings, objects and more:

Concept of Data Types
In programming, data types is an important concept.

To be able to operate on variables, it is important to know something about the type.

Without data types, a computer cannot safely solve this:

Escape Character:

var x = "We are the so-called \"Vikings\" from the north.";
The \ method is not the preferred method. It might not have universal support.
Some browsers do not allow spaces behind the \ character.

******************************************************

Strings Can be Objects
Normally, JavaScript strings are primitive values, created from literals:

var firstName = "John";

But strings can also be defined as objects with the keyword new:

var firstName = new String("John");

******************************************************

String Methods:

Both indexOf(), and lastIndexOf() return -1 if the text is not found.

Did You Notice?
The two methods, indexOf() and search(), are equal?

let = 34;


They accept the same arguments (parameters), and return the same value?

The two methods are NOT equal. These are the differences:

*The search() method cannot take a second start position argument.
*The indexOf() method cannot take powerful search values (regular expressions).

*The slice() Method
slice() extracts a part of a string and returns the extracted part in a new string.

The method takes 2 parameters: the start position, and the end position (end not included).

This example slices out a portion of a string from position 7 to position 12 (13-1):

Example 1
var str = "Apple, Banana, Kiwi";
var res = str.slice(7, 13):

Single Parameter example;

let x = 'da ya sahi dy kha mara sahii da'

x.search('sahi')
6 --- index value

let z = x.slice(6)

'sahi dy kha mara sahii da'

---------------------------------
Example 2:

Negative values ouput

let aa = "Apple, Banan, Graphs, Kiwi"
let bb = aa.slice(-8)

bb
'hs, Kiwi'

The substring() Method
substring() is similar to slice().

The difference is that substring() cannot accept negative indexes.

---------------------------------

*The substring() Method
substring() is similar to slice().

The difference is that substring() cannot accept negative indexes.

Example
var str = "Apple, Banana, Kiwi";
var res = str.substring(7, 13);

The result of res will be:
Banana

----------------------------------

Replacing String Content
*The replace() method replaces a specified value with another value in a string:

*The replace() method does not change the string it is called on. It returns a new string.
By default, the replace() method replaces only the first match:

Example:

let a = 'this is the main string'

let b = a.replace('main', 'aham')

console.log(b)
'this is the aham string'

--------------------------------------------------

*The replaceAll()

Example 1:
 
let x = 'get will soon, he will coming soon'

let z = x.replaceAll('soon')

console.log(z)
get will undefined, he will coming undefined

---------------------------------------------------

Example 2:

let x = 'Get will soon and he\'ll\ coming soon'

let z = x.replaceAll('soon', 'early')

console.log(z)
Get will early and he'll coming early

***************************************************
**************************************************

Coding practice

// single line comment
/*  multi-line comment */

Primitive Data Type:
A primitive data type is either a data type that is built into a programming language, 
or one that could be characterized as a basic structure for building more sophisticated data types.
Programmers will often be immediately familiar with the primitive data types used in coding,
which do not involve more sophisticated data sets for effective representation.

A regular expression is a sequence of characters that forms a search pattern.

----------------------------------------------------------
Data Types and Varaibes
JS provides 7 different data types.
undefined, null, boolean, string, symbol, number and object
*/
// let x = null;
// let y;
// console.log(x,y)

/* -------------------------------------------------------*/

// Escaping Literal Quotes in Strings
// Good practice 

// var myStr = 'I am a "double qouted string inside" qoutes! ';
// var myStrr = "I am a 'double qouted string inside' qoutes! ";
// var mystr = "I am a \"double qouted string inside\" qoutes! ";
// var mysstr = "I am a \\double qouted string inside\\ qoutes! ";
// var mysttr = "Firstline \t this is the beginning of new line "

// console.log(myStr, myStrr, mystr, mysstr, mysttr, mysttr, mysttr)

/*------------------------------------------------------------ */

/** Finding index of the specific position in Strings */


// let x = 'da ya sahi dy kha mara sahii da sahi'
// let y = x.search('sahi')
// let z = x.indexOf('sahi',15)
// let i = x.lastIndexOf('sahi')
// console.log(y,z,i)
   Output: 6 23 32
-----------------------------------------------------
** find the letter by index


var firstLetterOfFirstName = "";
var firstName = "Ada"

firstLetterOfFirstName = firstName [1];
 console.log(firstLetterOfFirstName);

-------------------------------------------------

/* Changing in String */

let x = "Jello World";
x = 'H' + x.slice(1,11)
console.log(x);
----------------------------------------------------

/** Finding index of the specific position in Strings */

// let x = 'da ya sahi dy kha mara sahii da sahi'

// let y = x.search('sahi')
// let z = x.indexOf('sahi',15)
// let i = x.lastIndexOf('sahi')
// console.log(y,z,i)

// ------------------------------------------------------

// Blank words
// function worldBanks (myNoun, myAdjective, myVerb, myAdverb){
//     var result = "";
//     result += "The " + myAdjective + " " + myNoun + " " + myVerb + " to the store " + myAdverb;
//     return result;
// }
// console.log(worldBanks("Dog", "Big", "run", "quickly"))
// console.log(worldBanks("bike","slow","flew","store"))
// -------------------------------------------------------

/**************** Array **********

// Store multiple values in Array
// every element in array is seprate by ','
// let ourArray = ['abbey', 47]
// console.log(ourArray)
-----------------------------------------.

***** Nested Array ****/
// Multidimentional Array

// let ourArray = [['React', 14],["Angular", 71]];
// console.log(ourArray)

// **** Access Array Data with Indexes ***/

// let ourArray = [10,20,30];
// let ourData = ourArray[0];
// console.log(ourData)
Output: [10]

// ------------------------------------

// let ourArray = [10,20,30];
// ourArray[1] = 45;
// console.log(ourArray);

// Output: [ 10, 45, 30 ]

//---------------------------------------.


 /** Access Multi-Dimensional Arrays with Indexes ***/
 
 var myArray = [
    [1,2,3],
    [4,5,6],
    [7,8,9],
    [
        [10,11,12],
        [   
            13, 
            14, 
            [15,16]
        ]
    ]
];
 
 var myData = myArray [3][1][2][1];
 
 
 console.log(myData);
----------------------------------------------.









