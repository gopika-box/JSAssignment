# JavaScript
## Assignment-2
### 1.	 What is a variable in JavaScript?
>  Variables in JavaScript are named containers used to store and manage data within a program. They allow you to hold different types of information, such as numbers, text, or objects, and can manipulate that data throughout your code. 
### 2.	 What are the variable naming conventions in JavaScript?

> - Variable names are case-sensitive
> - Variable names can be single character,  multiple character or alphanumeric. eg: a, abc, abc123
> - Camel case is the best naming convention. eg: userName, userLoggedIn
> -Variable names can't start with numbers and cannot have space in between.
> - Variable names cannot be keywords

### 3.	What is the difference between declaration, initialization, and re-assignment?
 Ans:   
`Declaration` is the process of creating a variable name in program memory.  
eg: let x;  
`Initialization` is the process of assigning a value to a variable.  
Eg: let x=10; or  
x=10;  
`Re-assignment` refers to changing the value of a previously initialized variable.  
let x = 10;  
x = 20;

### 4.	What are the different types of scope in JavaScript?
> Ans: `Global Scope:` Variables or functions declared outside of any function or block reside in the global scope. They are accessible from anywhere in the entire program.  
`Function scope:` variable declared inside a function.  
 `Block scope:`Variables that are declared inside the { } (curly braces) can only access inside that scope not from the outside of it.


### 5.	What does scope mean in the context of Javascript variables?
> Ans: Scope refers to the part of the code where a variable can be accessed. it determines whether a variable is accessable globally, within a function, or within a block.
### 6.	What are let, var, and const? What is the difference between them?
> Ans: All 3 are used to declare variables.  
`var` is function-scoped, and can be re-declared and reassigned.  
`let` is block-scoped, can be reassigned but not redeclared.  
`const` is also block-scoped, and must be initialized at the time of declaration, but can't be reassigned or re-declared.

### 7.	How do you determine the type of variable in javascript?
> Ans: typeof works for strings, numbers, booleans, objects, etc.   Using typeof() to check a variable's type:
```js 
let x=10;
console.log(typeof x); //number
```
> 
Note: typeof null returns "object"
### 8.	 What is hoisting? Explain with a code e.g.
> Ans: Hoisting in JavaScript means that variable and function declarations are moved to the top of their scope (function or global) before the code runs. This lets you use them earlier in the code, even before they are written.
```js
greet(); // Output: Hello from the function!

function greet() {
  console.log("Hello from the function!");
}
```
### 9.	 Create a greeting alert. Hint:(use => prompt, variable-message, alert)
```js
let name = prompt("What is your name?");
let message= "Welcome " +name;
alert(message);
```
### 10.	 Write some code so that the values of the below variables switch around.   Let a = 5, let b = 8. Switch the value so that a holds the value 8 and the variable b holds the value. 
```js
let a=5;
let b=8;
let temp=a;
a=b;
b=temp;
console.log("a = "+a);
console.log("b = "+b);
```


### 1.	: Variables defined with let cannot be redeclared.
a.	True
b.	False
> Ans: True
### 2.	 Select whether the below JS code is valid or not:

let x = "Hello Peter Doe";
let x = 0;  
a.	Valid
b.	Invalid
>  Ans: Invalid
### 3.	Select whether the below JS code is valid or not:

var x = "John Doe";
var x = 0;  
a.	Valid
b.	Invalid
> Ans: Invalid
### 4.	Variables defined with const cannot be Reassigned.	
a.	True
b.	False
> Ans: True
### 5.	Variables defined with const can be Redeclared.
a.	True
b.	False
> Ans: False
### 6.	 Select whether the below JS code is valid or not:

const PI = 3.141592653589793;
PI = 3.14;  
a.	Valid
b.	Invalid
> Ans: Invalid
### 7.	Select whether the below JS code is valid or not:

const PI = 3.141592653589793;
PI = PI + 10;  
a.	Valid
b.	Invalid
> Ans: Invalid
### 8.	A value must be assigned to a const variable when it is declared
a.	True
b.	False
> Ans: True
### 9.	 Select whether the below JS code is valid or not:

const PI;
PI = 3.14159265359;  
a.	Valid
b.	Invaid
> Ans: Invalid
### 10.	: Select whether the below JS code is valid or not:

const cars = ["Ford", "Honda", "BMW"];
cars[0] = "Nissan";  
a.	Valid  
b.	Invalid
> Ans: Valid
### 11.	Select whether the below JS code is valid or not:

const cars = ["Ford", "Honda", "BMW"];
cars = ["Toyota", "Skoda", "Audi"];  
a.	Valid  
b.	Invalid
> Ans: Invalid
### 12.	Select whether the below JS code is valid or not:

var x = 2;
var x = 3;  
a.	valid  
b.	invalid
> Ans: valid
### 13.	Select whether the below JS code is valid or not:

const x = 2;

{
const x = 3;
}

{
const x = 4;
}  
a.	Valid  
b.	Invalid
> Ans: Valid
### 14.	 What will be the console output of the below javascript code?

const a=34;
let b=56;
console.log(a=b);  
a.	Uncaught type error: Assignment to constant variable  
b.	56	  
c.	False  
d.	34

> Ans: a

