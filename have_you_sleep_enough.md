# Sleep Debt Calculator

Did you know that giraffes sleep 4.6 hours a day? We humans need more than that. <br>
If we don’t sleep enough, we accumulate sleep debt. In this project we’ll calculate if you’re getting enough sleep each week using a sleep debt calculator.

🤔💭🔢✖️🧮 <br>
The program will determine the actual and ideal hours of sleep for each night of the last week.<br>

Finally, it will calculate, in hours, how far you are from your weekly sleep goal.

#### Refactored code to make it faster and easier to read
```js
// Tell me your ideal sleep hours
let idealHours = 8;

//Tell me how much you slept each day, please
const monday = 10;
const tuesday = 8;
const wednesday = 8;
const thursday = 8;
const friday = 8;
const saturday = 8;
const sunday = 8;

const getActualSleepHours = () => {
  const totalSleepHours =
    monday + tuesday + wednesday + thursday + friday + saturday + sunday;
  return totalSleepHours;
};

const getIdealSleepHours = idealHours => idealHours *= 7;

const calculateSleepDebt = () => {
  const actualSleepHours = getActualSleepHours();
  const idealSleepHours = getIdealSleepHours(idealHours);
  if (actualSleepHours === idealSleepHours) {
    console.log(
      "You sleep " +
        actualSleepHours +
        " hours total and your ideal was " +
        idealSleepHours +
        " hours.\r\n You got the perfect amount of sleep!"
    );
  } else if (actualSleepHours > idealSleepHours) {
    console.log(
      "You sleep " +
        actualSleepHours +
        " hours total and your ideal was " +
        idealSleepHours +
        " hours.\r\n You got " +
        (actualSleepHours - idealSleepHours) +
        " hour(s) more sleep than needed."
    );
  } else {
    console.log(
      "You sleep " +
        actualSleepHours +
        " hours total and your ideal was " +
        idealSleepHours +
        " hours.\r\n You got " +
        (idealSleepHours - actualSleepHours) +
        " hour(s) less sleep than you needed this week. Get some rest!"
    );
  }
};

calculateSleepDebt();
```
