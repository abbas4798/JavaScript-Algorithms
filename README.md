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

======================

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


let x = 'da ya sahi dy kha mara sahii da sahi'
let y = x.search('sahi')
let z = x.indexOf('sahi',15)
let i = x.lastIndexOf('sahi')
console.log(y,z,i)
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

let x = 'da ya sahi dy kha mara sahii da sahi'
let y = x.search('sahi')
let z = x.indexOf('sahi',15)
let i = x.lastIndexOf('sahi')
console.log(y,z,i)

// ------------------------------------------------------

// Blank words
// function worldBanks (myNoun, myAdjective, myVerb, myAdverb){
  var result = "";
  result += "The " + myAdjective + " " + myNoun + " " + myVerb + " to the store " + myAdverb;
  return result;
  }
  console.log(worldBanks("Dog", "Big", "run", "quickly"))
  console.log(worldBanks("bike","slow","flew","store"))
// -------------------------------------------------------

/**************** Array **********

// Store multiple values in Array
// every element in array is seprate by ','
// let ourArray = ['abbey', 47]
// console.log(ourArray)
-----------------------------------------.

***** Nested Array ****/
// Multidimentional Array

let ourArray = [['React', 14],["Angular", 71]];
console.log(ourArray)

// **** Access Array Data with Indexes ***/

let ourArray = [10,20,30];
let ourData = ourArray[0];
console.log(ourData)
Output: [10]

// ------------------------------------

let ourArray = [10,20,30];
ourArray[1] = 45;
console.log(ourArray);
Output: [ 10, 45, 30 ]

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

Code Examples :

// Boolen Data type

var abb = true;

if(abb){
    console.log("this is true statement")
}
else{
    console.log("this is false statement")
}

// -------------------------
  
/* Adding . values */

  let x = 4.5;
  let y = 3.3;
  let z = x+y;
  console.log(z);

// -------------------------

//*** Access Multi-dimensional Arrays **//
 let myArray = [
   [1,2,3],
   [4,5,6],
   [7,8,9],
   [10,11,12],
       [
            [13,14,15],
            [18,19,20,
	    [21,22,
            [23,24]
        ]
         ],
        16,
        17
       ]
           ];
 let myData = myArray[4][1][3][2][1];
console.log(myData)

// ------------------------------------------


const index = ourArray.findIndex((item) => item.some((item) => item === 'goat'))
ourArray[index] = ourArray[index].filter((item) => item !== 'goat')


console.log(ourArray);

———————————————————————

const a = [['a','b','c'],['d','e','f'], 2, 1, {a:"b"}];

const index = a.findIndex((item) => {
return item.length === undefined && typeof item === 'object'
    console.log(item.length === undefined && typeof item === 'object' )
} )

a[index] = a[index].filter((item) => item !== "e")
a[4] = {b : a[4].a}

// console.log(a[4])

// -----------
Let = a[“a” , ”b” , “c”] , 1 , 2 {a: ‘b’};
a[3] = ['a','b','c']
console.log(a)

——————————————————————-
——————————————————————-

11 January 2023

/** Using of Shift function**/
// It's remove the first element of array

// let myArray = ["apple", "orange", "banana"]
// myArray.shift();
// console.log(myArray)

OUTPUT: [ 'orange', 'banana' ]

// ---------------------------------

/* Using of Unshift method()***/
It's add new element in our starting position of Array

let myArray = ["apple", "orange", "banana"]
myArray.unshift('graphs');
console.log(myArray)

OUTPUT: [ 'graphs', 'apple', 'orange', 'banana' ]

Example:

let myArray = ["apple", "orange", "banana"]
myArray.unshift('graphs');
myArray.push('last')
console.log(myArray)

OUTPUT: [ 'graphs', 'apple', 'orange', 'banana', 'last' 

———————————————————

Object:

Object is similar to Map —both let you set keys to values, retrieve those values, delete keys, and detect whether something is stored at a key


// ------------------------------------


JS FUNCTION

// Function ourReusableFunction(){
//     console.log("this is normal function")
// }
// Functions are the most important weapon you have in your arsenal, but you need to understand very well that a function is a first-class object, they are treated like an object, also a function can be referred by variables, declared with literals and even passed as a function.

// Four parts of a function (or syntax)

// 1) The function keyword.
// 2) An optional name ( this is also because it can be anonymous ).
// 3) A list of parameters names enclosed in parentheses.
// 4) The statement enclosed in braces.

//Function declaration

// One way to define a function is like the following code, keeping the four parts of a function, a function declaration is well known too as a function statement.

// The return statement returns a value from the parameter. you can call the function by just mentioning its name, followed by the arguments in the parentheses.

// Remember that if you don’t return nothing in the parameters part, the value will be “undefined”

————————————————

Parameter and Argument

The words parameters and arguments are well interchangeably, this is because sometimes we used wrong when we talk with other developers, but there is a rule of gold for distinguishing them.

Parameter
This is used only to define a function, also they are called formal parameters and formal arguments, I will show you an example

￼

Argument
This is used only to invoke a function, also they are called actual parameters and actual arguments, I will show you an example
￼
￼
——————————————————————

The use
The key principles to use functions is modularity and reusability, because each function does its own work, but this can maintain your code rather well organized, and also takes care of your libraries and call your functions many times you want!


The roles
A function can play several roles

* As a literal function We can call a function in a direct way, and it will work as a normal function. The names of a normal function start with lowercase letters.
￼
￼
Calling the function as a literal

* Method You can make a function in a property of an object, which turns in to a method. you can invoke this function via an object. The names of methods start with lowercase letters.
￼
￼
Function as a method ( knowledge )
￼
￼
Calling the function as a method
* 		Constructor You can call a function via the new operator. which turns it into a constructor, a factory for objects. The names of methods start with uppercase letters.
￼
￼

Calling the function as a constructor

————————————————————————————————————————————.
4
Function expressions

There is another way to define a function, which is the function expression, in this particular way you can produce a value, let see an example.
￼
￼
Function expression

This type assigned the result of a function expression to a variable, which we could be called it later with that variable.

——————————————————————————————————————————.

Anonymous functions
From the previous example, you can see, that the name of the function is the name of the variable, this is because we don’t insert a name of the function statement, these are called the anonymous function (a function without a name). In other words.

Functions stored in variables do not need function names. They are always invoked (called) using the variable name.

———————————————————————————————————————————.
The war
There is a war between the functions declaration and function expression, the war is the argument for which is better.
I have always been ask, which is better?, what function definition do I prefer?, do I combine both?
I always answer they are basically the same dude! but function declarations have two advantages over function expressions.
* 		They are hoisted and they have a name which for me is a lot better! thig about it! ;)

—————————————————————————————————————————.


Define a function
If you get all the way through here, you already know there are three ways to create a function.
* 		The function expression
* 		The function declaration
* 		The constructor Function()

———————————————————————————————————————————.

Scoping
This is a very interesting thing, and actually I would like to make a whole chapter about this, but for now, you should know that a variable’s scope is the context in which the variable exists. This means from where to where you can access a variable and whether you have access to the variable in that context
The scoping can be defined as global or local.

Global
All the variables that you declare, is by default defined in global scope, in the personal matter of each developer this is very annoying language design decision take in JavaScript. this is because as a global variable is visible from all the scopes and therefore can be modified in any scope
The way you can create a global variable is
* 		Declare the variable outside a function with a var statement
* 		Omit the var statement while declaring a variable. this is kinda headache because if you omit or forgot to put the var statement its turn into a global variable by default
* 
Local
Unlike most programming languages, JavaScript does not have a block-level scope like Perl, Python or PHP… (these means variables scoped surrounding in curly brackets). in order to get the local scope, we need to declare the variable in the function

———————————————————————————————————————————.

Hoisting
I know guys, for the beginner’s dudes this word maybe a little bit scary, but no worries, the thing you need to understand is “hoisting is moving to the beginning of a scope”

￼
Completely hoisted function

￼
Completely hoisted variable XD

￼
The error from trying hoist a function expression



—————————————————————————————————————————.


Coding mini projects :

/* Simple- normal function */

function Myfun () {
     console.log("hello world");
 }
 Myfun();
 Myfun();
 Myfun();

OUTPUT: 
hello world
hello world
hello world

---------------------------------

/* Simple function set parameters, then invoke fun and pass arguments */
parameters are variables that act as place holders for the values

function Myfun(a,b){
     return a + b;
 }
 console.log(Myfun(1,5));

OUTPUT: 6

---------------------------------

/* GLobal Scope and Function

 Scope refers to the visibility of variables 
 variables which are defined outside of a function block have global scope.
 Global scope mean they can be seen everywhere in our javascript code.
 So, normally if you do use a var keyword, since this is within a function , it will be scoped to that function. */
 
 var myGlobal = 7;
 
 function fun1(){
   oopGlobal = 4; // this variable invoke by globally
   var localVariable = 8; //
   }
 
   function fun2(){
      var output = "";
      if (typeof myGlobal != "undefined"){
          output += "myGlobal " + myGlobal ;
      }
      if( typeof oopGlobal != "undefined"){
          output += " oopGlobal " + oopGlobal;
      }
       if( typeof localVariable != "undefined"){
          output += " localVariable " + localVariable;
      }
      console.log(output);
  }
  fun1();
  fun2();

OUPUT: myGlobal 7 oopGlobal 4
 
----------------------------------------------
 
/* Local Scope and Funtion
Variables which are declared within function as well as the function paramteres have local scope.
That mean they're only visible from within the function.

function LocalScope (){
 var myVar = 5;
   console.log(myVar);
}
 LocalScope();
 console.log(myVar)

OUTPUT: 5 & error message

------------------------------------------------

/* Global vs Local Scope in Funciton

 It is possible to have both local and global variables with in the same name.

Example: 1
 var outerWear = "T-Shirt ";
 var outerWearr = "Coat ";
 
 function myOutFit (){
  return outerWear + outerWearr;  
  };
 
  console.log(myOutFit());

OUTPUT: T-Shirt Coat 
 
—————————————————————————
Example: 2

 var outerWear = "T-Shirt ";
 
 function myOutFit (){

   var outerWear = "Sweeter"	 // show this value now

   return outerWear;   // we can return a value form function with this return statement.
 };
 
 console.log(myOutFit());
 console.log(outerWear); 		// this show 'T-shirt'

OUTPUT: Sweeter
		 T-Shirt 

 
—————————————————————————

let Global = "This is outer variable"

function fun1() {
   var Global1 = "1st"
    return Global1;
}

function fun2() {
    var Global = "2st"
    return Global;
}

function fun3() {
    var Global = "3st"
    return Global;
}

function fun4(Global1) {
    var Global = "4st";
    return Global1 + Global;
}

console.log(fun4('passing_data through argument '), fun3(), fun2(), fun1())

OUPUT: passing_data through argument 4st 3st 2st 1st

——————————————————————————.

Return value from a function

Example: 1

function a (a){
    return a - 12
}
console.log(a(14))

OUTPUT: 2

——————————————————————————.

Example: 2

var changed = 0;

function change (num){
    return (num + 2) / 2;
}
console.log(change(3))

OUTPUT: 2.5

——————————————————————————.

Example: 3

var changed = 0;

function change (num){
    return (num + 2) / 2;
}
changed += change(5);
console.log(changed)

OUTPUT: 3.5

——————————————————————————.

/* Assigning new value in array */
let x = [1,2,3,4,5,6]
x[1] = 9
console.log(x);

——————————————————————————.
Iterable is an object which can be looped over or iterated over with the help of a for loop. Objects like lists, tuples, sets, dictionaries, strings, etc. are called iterables. In short and simpler terms, iterable is anything that you can loop over.

Array + List


/* JSON.stringify() method */

// In Computer Science a cue is an abstract data structure where items are kept in order.
// New items can be added to the back of the cue and old items are taken off from the front of the cue.
// We are going to simulate that right now, 

Example: 1

const obj = {name: "dev",
             today: new Date(),
             city : "Lhr",
             location:4747};
console.log(typeof obj)
const myJSON = JSON.stringify(obj);
console.log(typeof myJSON)

OUTPUT: object
        string


// ---------------------------

Example: 2

let obj = {name: "John", age: 30};
console.log(typeof obj);
let str = JSON.stringify(obj, null, 2);
console.log(typeof str);

OUTPUT: object
                 string
// ---------------------------

Example: 3

let v = [1,2,3,4,5];
let x = JSON.stringify(v);
console.log(typeof x)

------------------------------

JS 7 types of Data types

let a = [1,2,3];
let b = "akjjk";
let c = {a:1, b:2, c:3};
let d= 47;
let e = true;
let f = null;
let g;

console.log(typeof(a))
console.log(typeof(b))
console.log(typeof(c))
console.log(typeof(d))
console.log(typeof(e))
console.log(typeof(f))
console.log(typeof(g))

OUTPUT:
object
string
object
number
boolean
object
undefined



——————————————————————————.
*************************************************


13 January 2023

Pseudocode


Description
In computer science, pseudocode is a plain language description of the steps in an algorithm or another system. Pseudocode often uses structural conventions of a normal programming language, but is intended for human reading rather than machine reading.

Format

Pseudocode is an artificial and informal language that helps programmers develop algorithms. Pseudocode is a "text-based" detail (algorithmic) design tool. The rules of Pseudocode are reasonably straightforward. All statements showing "dependency" are to be indented.

————————————————.

Spread syntax (...)

Spread syntax can be used when all elements from an object or array need to be included in a new array or object, or should be applied one-by-one in a function call's arguments list. There are three distinct places that accept the spread syntax:

Function arguments list (myFunction(a, ...iterableObj, b))
Array literals ([1, ...iterableObj, '4', 'five', 6])
Object literals ({ ...obj, key: 'value' })


// * Spread operator/ Rest operator
// add the elements of an existing array into new array
// Pass elements of an array as arguments to a function
// copy arrays
// concatenate array


// Example: 1

// const numbers = [1, 2, 3];
// function sum(x, y, z) {
//   return x + y + z;
// }

// console.log(sum(...numbers));

// OUTPUT: 6

// ------------------------------------

// Example: 2

//Aizaz example:

// const obj = { a: 'aizaz', b: 'waheed' }
// let b = {
// a: obj.a + " " + obj.b,
//     ...obj
// }

// console.log(obj)

// OUTPUT: { a: 'aizaz', b: 'waheed' }

// -------------------------------------

// Example: 3

//add the elements of an existing array into a new array
// let x = ["front-end", "backend"];
// let y = ["AWS", "Azure", ...x, "Google cloud"]
// console.log(y)

// OUTPUT: [ 'AWS', 'Azure', 'front-end', 'backend', 'Google cloud' ]

// ----------------------------------------

// Example: 4

//pass elements of an array as arguments to a function
// let y = [2,2,2];
// x(...y);

// function x (a,b,c) {
// console.log(a+b+c)
// }

// OUTPUT: 6

// ------------------------------------------

// Example: 4

////copy array
// let y = [2,2,2,3]; // ignore last fourth element cause                     funtion have just 3 argument items
// x(...y);

// function x (a,b,c) {
// console.log(a+b+c)
// }

// OUTPUT: 6

// -------------------------------------------

// Example: 5

//copy array / passing new element
// let x = [1,2,3,4];
// let y = [...x];
// y.push(5)
// console.log(x);
// console.log(y);

// OUTPUT: [ 1, 2, 3, 4 ]
// [ 1, 2, 3, 4, 5 ]
// ----------------------------------------------

// Example: 6

//concatenate array
// let x = ['a','b','c'];
// let y = ['d','e','f'];
// // console.log(x.concat(y))x;
// x = [...x, ...y]
// console.log(x)

// OUTPUT: [ 'a', 'b', 'c', 'd', 'e', 'f' ]
// --------------------------------------------------

/* REST Opearator */

// REST: condense multiple elements into a array.
// the rest operator is looks exactly like spread operator. it's just 3 dots but it's bascially the opposite of the spread operator.
// the spread operator spreads or expands an array to it's elements but the rest operator collects multiple elements and condenses into a single array element.

// Example: 1

// function xyz (a,...b){
//     return b.map(function(item) {
//         return a + item;
//     });
// };

// let y = xyz(2,2,2,6);
// console.log(y);

// OUTPUT: [ 4, 4, 8 ]

// --------------------------------


const list = [
    {
    firstName: "Aizaz",
    lastName: "Waheed",
    email:"aizazwaheed@gmail.com"
      },
    
    {
    firstName: "Ali",
    lastName: "Ahmad",
    email:"aliahmad@gmail.com"
      },

    {
    firstName: "Muhammad",
    lastName: "Hassan",
    email:"Muhammadhassan@gmail.com"
        },

    { 
    firstName: "Faraz",
    lastName: "Ahmad",
    email:"farazahmad@gmail.com"
      },

    {
    firstName: "Usman",
    lastName: "Ashraf",
    email:"usmanashraf@gmail.com"
      }
    ]
    
    const data = list.map((item) => {
        return {...item, firstName: item.lastName, lastName: item.firstName}
    })
    console.log(data);
    
//   ##############
    
     let x = list.map(getFullName);
    
    function getFullName(item){
        return {
            ...item
        }
    }
    console.log(x)
    
    // -----------------------------------------


















