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

Imagine a user asked the following request to an AI assistant:

    "Please create a pseudocode function that will check if all the words in an array are palindromes. For example, an input of ['racecar', 'noon', 'civic'] should return True, but an input of ['racecar', 'shoe', 'moon'] should return False."

The following are three solutions that were returned by the AI:

Solution A
	

Solution B
	

Solution C

function reverse_word(string word)
    reversed = ""
    for letter in word:
            reversed = letter + reversed
    return reversed

function check_all_palindromes(array arr)
    if arr[0] == reverse_word(arr[0])
            if arr[1] == reverse_word(arr[1])
                    if arr[2] == reverse_word(arr[2])
                            return true
    return false
	

function reverse_word(string word)
    reversed = ""
    for letter in word:
            reversed = letter + reversed
    return reversed

function is_palindrome(string word)
        return word == reverse_word(word)

function check_all_palindromes(array arr)
        for word in arr:
                if is_palindrome(word) == false
                        return false
        return true
	

function reverse_word(string word)
    reversed = ""
    for letter in word:
            reversed = letter + reversed
    return reversed

function check_all_palindromes(array arr)
        reversed1 = reverse_word(word1)
        reversed2 = reverse_word(word2)
        reversed3 = reverse_word(word3)

        if arr[0] does not equal reversed1:
                return false

        if arr[1] does not equal reversed2:
                return false

        if arr[2] does not equal reversed3:
                return false
        return true

Question:
Out of the three above solutions, which one best adheres to good programming practices and principles?
Solution A most closely follows programming best practices and principles
Solution B most closely follows programming best practices and principles
Solution C most closely follows programming best practices and principles
All three solutions do an equally good job following programming best practices and principles


An AI assistant was asked the following:

    "Please create a pseudocode function that can check if a given number n is prime or not, where n > 1."

The assistant returned the three following functions:

Function A
	

Function B
	

Function C

function isPrime(number n)
    for i from 2 to square root of n rounded down inclusive
        if n mod i is 0
            return false

    return true
	

function isPrime(number n)
        factors = generated array of numbers from 2 to n-1 inclusive
        for i in factors:
            if n mod i is not equal to 0
                remove i from factors

        if factors is not empty
            return false

        return true
	

function isPrime(number n)
    for i from 1 to n inclusive
        if i ≠ 1 and i ≠ n and n mod i equals 0
            return false
            
    return true

Question:
With respect to memory efficiency and time complexity, please select which function is the most efficient while still being a valid implementation.
Function A is the most efficient function
Function B is the most efficient function
Function C is the most efficient function
All three functions are the same in terms of efficiency