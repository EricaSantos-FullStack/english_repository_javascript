# The 🎱 Magic Eight Ball

You’ve learned a powerful tool in JavaScript: control flow! <br>
It’s so powerful, in fact, that it can be used to tell someone’s fortune.<br>
In this project we will build a Magic Eight Ball using control flow in JavaScript.<br>
The user will be able to input a question, then our program will output a random fortune.

```js
// empty string in the user name and question
let userName ='';
const userQuestion = '';
// random number with Math.random(), however it gives a float number. To get a integer number, make it round with Math.floor()
let randomNumber = Math.floor(Math.random() * 8);
//this variable will have the answers of the magical eight ball
let eightBall = '';

switch(randomNumber){
  case 0:
  eightBall = 'It is certain';
  break;
  case 1:
  eightBall = 'It is decidedly so';
  break;
  case 2:
  eightBall = 'Reply hazy try again'
  break;
  case 3:
  eightBall = 'Cannot predict now'
  break;
  case 4:
  eightBall = 'Do not count on it'
  break;
  case 5:
  eightBall = 'My sources say no'
  break;
  case 6:
  eightBall = 'Outlook not so good'
  break;
  case 7:
  eightBall = 'Signs point to yes'
  break;
}

userName ? console.log(`Hello, ${userName}!`) :  console.log("Hello!");

console.log(`Your question is ${userQuestion}`);
console.log(`Your answer is ${eightBall}`);
```

#### Output
```
Hello, Erica!
Your question is Will I be rich?
Answer: Signs point to yes
```
