# JavaScript
## Assignment 4

### 1.	Write a chained if / else-if statement to fill in the following conditions

val  < 5  =>  Tiny  
val  < 10  =>  Small  
val  < 15  =>  Medium  
val  < 20  => Large  
val  >= 20  => Huge 

```js
if(val < 5){
    console.log("Tiny")  }
else if(val < 10){ 
    console.log("Small") }
else if(val < 15>){
     console.log("Medium") }
else if(val <20){
    console.log("Large") }
else {
    console.log("Huge")
}
```

### 2.	Use the switch case and create an application with the following roles.

admin => gets full access  
subAdmin => gets access to create and delete courses  
testPrep => gets access to create and delete tests  
user => gets access to consume contents  

```js
let role = "admin"
switch(role)
{
    case "admin":
        console.log("Gets full access");
        break;
    case "subAdmin":
        console.log("gets access to create and delete courses");
        break;
    case "testPrep":
        console.log("gets access to create and delete tests");
        break;
    case "user":
        console.log("gets access to consume contents");
        break;
}
```
### 3.	Check if the person is eligible for voting
```js
let age=20;
if(age>=18){
    console.log("Eligible");
}
else{
    console.log("Not eligible");
}
```
### 4.	Check if the person has a fever (normal temperature: 98.6F)
```js
let temp=80;
if (temp> 98.6){
    console.log("Fever")
}
else{
    console.log("temperature is normal")
}
```

### 5.	Check if someone has normal temperature: Normal temp= (98 to 98.9)
98.1 => normal
99 => not normal
97.9 => not normal
```js
let temp= 99
if(temp >=98 && temp<=98.9){
    console.log("Normal");
}
else if(temp >=99)
{
console.log("Not Normal");
}
else{
    console.log("Not Normal");
}
```
### 6.	You need to have 75% attendance to write the exam. Take the total number of classes and the number of attendances from the student and tell him if he can write the exam

```js
let Tclass= prompt("Enter total number of class: ");
let attend_class = prompt("Enter the no of class attended: ")
let attendence = attend_class*100/Tclass;
if (attendence> 75)
{ console.log("eligible to write exam");
}
else
{
    console.log("not eligible");
}
```



### 7.
```js
if(5>4){  
Console.log(“First if”)  
}  
if(10 >= 6){
Console.log(“Second if”)
}
```
What will the output of the above code be?  
Ans:   
> First if  
Second if


### 8.
```js
if(true){
console.log(“1”)
}
if(false){
console.log(“2”)
}
if(true){
console.log(“3”)
   }
   ```
What will the output of the above code be?
>1  
3
### 9.	What will be the output of the code below?
```js
let a = 50
let b = 50
if(a >= 50){
  console.log("a scored half");
  a = a + 1
}
if(b >= 50){
  console.log("b scored half");
  b = b + 1
}

console.log(a + b);

```
Ans:
> a scored half  
b scored half  
102


