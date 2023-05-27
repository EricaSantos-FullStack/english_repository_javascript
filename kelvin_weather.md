# Kelvin Weather

✨ Exercice made during CodeCademy studies + learning technical English for Technology ✨

Deep in his mountain-side meteorology lab, the mad scientist Kelvin has mastered weather prediction.<br>
Recently, Kelvin began publishing his weather forecasts on his website. However there’s a problem: All of his forecasts describe the temperature in Kelvin.<br>
With our knowledge of JavaScript, let’s convert Kelvin to Celsius, then to Fahrenheit.

#### 🛰 Also Convert celsius to the Newton scale 

```js
//Forecast today is 293 kelvin
let kelvin = 293;
//Celsius is 273 degrees less than kelvin
let celsius = kelvin - 273
// equation to calculate Fahrenheit
// Math.floor() method to round the answer
let fahrenheit = Math.floor(celsius * (9/5) + 32);
//equation to calculate Newton Scale
let newton = Math.floor(celsius * (33/100))

console.log(`The temperature is ${fahrenheit} degrees Fahrenheit`)

console.log(`The temperature is ${newton} degrees in the Newton Scale`)

console.log(`The temperature is ${celsius} degrees Celsius`)
```

#### Funny and interesting way to practice JavaScript with tempeture
