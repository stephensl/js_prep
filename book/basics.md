Data Types in JS. 

**Primitives**
- String
- Number
- Undefined 
- Null 
- Boolean
- Symbol
- BigInt

*Every type that is not a primitive type is an **object type**.*


Data types can be represented by literals. Literals are notation that let you represent a fixed value in source code. 

'hello' --> string literal
3.14 ---> numeric literal
true --> boolean literal
{ a: 1, b: 2 } --> object literal
[ 1, 2, 3 ] --> array literal
undefined --> undefined literal


String interpolation: 

`5 plus 5 equals ${5 + 5}`

use backticks and ${}


implicit coercion. 

`console.log('5' + 10);`

= '510'.

Every `+` expression that has a string operand produces a string result no matter the other operand. 


console.log(Number('5') + 10)


Scope: 

variables declared with let or const have block scope. 



## Functions

base syntax for declaration: 

```js
function funcName() {
  func_body;
}
```

```js
function say() {
  console.log("Hi!");
}
```


or function expression 

```js
let greetPeople = function() {
  console.log("Good morning!");
}

greetPeople();
```

functions may be called before declared, but function expressions must be declared prior to invoking.


Arrow function syuntax

```js
let greetPeople = () => console.log("Good morning!");

greetPeople();
```

another example array function: 

```js
let add = (a, b) => a + b;
```

implicit return when the arrow function body contains a single expression that is not itself surrounded by curly braces. 
