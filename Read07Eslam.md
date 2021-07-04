# Functions in JavaScript

### what is Functions?
Functions are one of the fundamental building blocks in JavaScript. A function in JavaScript is similar to a procedure/a set of statements that performs a task or calculates a value, but for a procedure to qualify as a function, it should take some input and return an output where there is some obvious relationship between the input and the output. To use a function, you must define it somewhere in the scope from which you wish to call it.

### Why use it ?

- code reusability
- less coding

### How use it ?

*Functions need to be declared **before** they can be invoked*


## Defining Functions

* There are Two ways to define function :
**Declaration Functions**  and **Expression Functions **

**1. Declaration Functions : **
 As shown in the following example, it consists of the function keyword, followed by: 

- The name of the function.
- A list of parameters to the function, enclosed in parentheses and separated by commas.
- The JavaScript statements that define the function, enclosed in curly brackets, {...}.

  

 ```
 function square(number) {
  return number * number;
}

 ```

 **2. Expression Functions :**
The function keyword can be used to define a function inside an expression. The main difference between a function expression and a function declaration is the function name, which can be omitted in function expressions to create anonymous functions. 


**Important Note: **  You can't use function expressions before you create them.

the function could be defined as 

```
const square = function(number) { return number * number }
var x = square(4) // x gets the value 16
```

## Calling functions
Defining a function does not execute it. Defining it names the function and specifies what to do when the function is called.

Calling the function actually performs the specified actions with the indicated parameters
