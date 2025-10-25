# JavaScript
## Assignment 6

### 1.	Write short notes on Array methods with a code example
### •	push()
The push() method adds a new element to an array (at the end).
It also return the length of new array.
```js
const arr =['a','b','c'];
len =arr.push('d');
console.log(arr);
console.log("len =",len);
```
Output: [ 'a', 'b', 'c', 'd' ]   
len = 4

### •	pop()

The pop() method removes the last element from an array, returns the value that was "popped out".
```js
const arr =['a','b','c'];
popped =arr.pop();
console.log(arr);
console.log("Popped value =",popped);
```
[ 'a', 'b' ]  
Popped value = c
### •	shift()
The shift() method removes the first array element and "shifts" all other elements to a lower index.The shift() method returns the value that was "shifted out"
```js
const arr =['a','b','c'];
shifted =arr.shift();
console.log(arr);
console.log("Shifted out =",shifted);
```
[ 'b', 'c' ]  
Shifted out = a
### •	unshift()
The unshift() method adds a new element to an array (at the beginning), and "unshifts" older elements.  
returns the new array length.
```js
const arr =['a','b','c'];
len =arr.unshift('d');
console.log(arr);
console.log("len =",len);
```
[ 'd', 'a', 'b', 'c' ]  
len = 4

### •	includes()
The includes() method returns true if a string contains a specified string.
```js
let str = "hello world"
console.log(str.includes("hello"))
```
true
### •	toString()
The toString() method returns the elements of an array as a comma separated string.
```js
const a=[1,3,5]
const c=a.toString()
console.log(c);
```
1,3,5

### •	reverse()
The reverse() method reverses the elements in an array.
```js
const arr =['a','b','c'];
arr.reverse();
console.log(arr);
```
[ 'c', 'b', 'a' ]
### •	join()
The join() method also joins all array elements into a string.Similar to toString() but we can select the seperator.
```js
const a=[1,3,5]
const c=a.join('*')
console.log(c);
```
`1*3*5`

### •	concat()
The concat() method creates a new array by merging (concatenating) existing arrays.
```js
const a=[1,3,5]
const b=[2,4,6]
const c=a.concat(b)
console.log(c);
```
[ 1, 3, 5, 2, 4, 6 ]
### •	flat()
The flat() method creates a new array with sub-array elements concatenated to a specified depth.
```js
const myArr = [[1,2],[3,4],[5,6]];
const newArr = myArr.flat();
```
[ 1, 2, 3, 4, 5, 6 ]
### •	slice()
The slice() method slices out a piece of an array into a new array.
```js
let text = "Hello world!";
let result = text.slice(0, 5);
console.log(result);
```
Hello
### •	splice()
used to change the contents of an array by removing, replacing, or adding elements in place.  
syntax:  
array.splice(start,delete_count,valuesToAdd)
```js
let arr = [1,2,3]
arr.splice(1,0,5,6)
console.log(arr);
arr.splice(1,2)
console.log(arr);
```
[ 1, 5, 6, 2, 3 ]
[ 1, 2, 3 ]
### •	sort()
The sort() method sorts an array alphabetically.
```js
const arr =[ 'c', 'b', 'a' ];
arr.sort();
console.log(arr);
```
[ 'a', 'b', 'c' ]
### •	fill()
fills the elements with a certain value  
syntax:  
array.fill(value,start,end)
```js
let arr = [1,2,3,4,5]
arr.fill(0,1,3);
console.log(arr);
```
[ 1, 0, 0, 4, 5 ]












