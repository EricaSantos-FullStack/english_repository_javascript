# Dog Years

✨ Exercice made during CodeCademy studies + learning technical English for Technology ✨

Dogs mature at a faster rate than human beings. We often say a dog’s age can be calculated in “dog years” to account for their growth compared to a human of the same age. In some ways we could say, time moves quickly for dogs — 8 years in a human’s life equates to 45 years in a dog’s life. How old would you be if you were a dog?

Here’s how you convert your age from “human years” to “dog years”:

- The first two years of a dog’s life count as 10.5 dog years each.
- Each year following equates to 4 dog years.

Before you start doing the math in your head, let a computer take care of it! <br>
With your knowledge of math operators and variables, use JavaScript to convert your human age into dog years.

```js
// writting down my age
let myAge = 21;
let name = "Erica";
// method to get your name with all lower case letters
let myName = name.toLowerCase();
// The first two years of a dog’s life count as 10.5 dog years each
let earlyYears = 2 * 10.5;
//logic: Since we already accounted for the first two years, subtract 2 from myAge. 
//Each year following equates to 4 dog years, so multiply the laterYears by 4
let laterYears = (myAge - 2) * 4;
// Total of years counting the first 2 years and the rest
let myAgeInDogYears = earlyYears + laterYears;

console.log(`My name is ${myName}. I am ${myAge} years old in human years which is ${myAgeInDogYears} years old in dog years.`)

```
