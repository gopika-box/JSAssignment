# JavaScript
## Assignment 5
### 1.	Write short notes on string methods with code examples
#### •	toLowerCase()
 - String is converted to lower case with toLowerCase()
 ```js
 let txt1 = "Hello World!";      
 let txt2 = text1.toLowerCase();
 //output: hello world!
 ```
#### •	toUpperCase()
 - String is converted to upper case with toUpperCase()
 ```js
 let txt1 = "Hello World!";      
 let txt2 = text1.toUpperCase();
 //output:
 ```
#### •	substring()
- is used to extract a portion of a string between two specified indexes.
```js
let str = "JavaScript";
console.log(str.substring(0, 4));
//output: Java
```
#### •	replace()
- to replace a specified value with another value in a string.
```js
let text = "i like java !";
let newText = text.replace("java","javascript");
//output:i like javascript!
```
#### •	trim()
- to remove whitespace from both sides of a string.
```js
let text1 = "  Hello World!  ";
let text2 = text1.trim(); 
//output: Hello World!
```
#### •	split()
- used to split a string into an array of substrings based on a given separator.
```js
let str = "apple,banana,mango";

let result = str.split(",");
//output: ["apple", "banana", "mango"]

```
#### •	slice()
- This method extracts a section of a string or array and return it as a new string or array, without modifying the original content.
```js
let str= "Javascript";
console.log(str.slice(0,4))
//output: "Java"
```

### 2. Create a simple app that takes the user’s name and greets him/her after capitalizing the first letter of the user’s name and changing the rest of the letters into lowercase (toUpperCase(), toLowerCase(), slice(), length property, string concatenation)

```js
let name = prompt("Enter you name:");
let len = name.length;
let firstLetr = name.slice(0,1).toUpperCase();
let restOfLetters = name.slice(1,len).toLowerCase();
let fullname = firstLetr + restOfLetters;
alert(`Good Morning ${fullname}`);

```

### 3.	Write some JavaScript code to create a prompt where the user can enter a long text, such as a paragraph from a blog post, and you will tell them how many characters remain out of either 20 characters. The output you should get should be something like “You have written 12 chars and you have 20 – 8 characters left”
```js
let comment = prompt("Enter you comment")
let countchar = comment.length;
let remain = 20 - countchar;
alert(`you have entered ${countchar} chars , and you have ${remain} char left`)
```

### 4.	Create a prompt that takes a comment from the user and, sends an alert after cutting the comment down to only 15 chars
```js
 let comment = prompt("Enter you comment") 
 alert(comment.slice(0,16)+"...")
```
