---
layout: step
number: 9
part: 1
title: Loops
permalink: step9/

---
People have always been lazy, but sometimes it moves progress forward! We
don't like to repeat the same boring actions again and again, so we look
for ways to avoid it. Programming is the same.

For example, if I want to print 'JavaScript is
awesome!' 10 times, what are my options? Of course, I can type ten lines of
console.log('JavaScript is awesome!'), but I can also tell the computer to
repeat it instead of me writing it 10 times!
For this we have loops.
Each loop should have three main things:
- a starting point
- a condition (finishing point)
- a counter (a step)
If you miss one of these, you can get into an infinite loop!
Let's look into different looping structures.


## While Loops

'While' loop will do an action forever until some condition is met.

```javascript
// starting point
var number = 0;
while (number < 10) {
    // 'less than 10'' is a condition (finishing point)
    console.log('JavaScript is awesome!');
    number = number + 1;
    // + 1 is a counter/size of the step
}
```

## For Loops

'For loops are very similar to the 'while loop'. In a for loop, you
declare a counter in the statement.

```javascript
var i;
for (i = 0; i <= 5; i = i + 1) {  // (starting point; condition; step)
    console.log('Purr');
}
```


## Iterating Through Arrays

Now we know about loops, I want to use each value from my animal list
and express my love for each. How shall I do it?
We can use a 'for loop' to iterate through our array and get each value
from it.
Note: i++ is another way of writing i = i+1.


```javascript
var animals = ['cats', 'dogs', 'horses'];
for(var i = 0; i < animals.length; i++){
    console.log('I love ' + animals[i]);
}
```

## Loops and Logic

Let's bring loops together with the if/else statements we learned in
learlier, and make something interesting.
Let's count from 10 to 0 and log all the numbers. But, when we get to the
middle (5) print 'Woohoo, we are in the middle!'.

```javascript
for (var i = 10; i >= 0; i = i - 1) {
    if (i === 5) {
        console.log('WooHoo, we are in the middle!');
    } else {
        console.log(i);
    }
}
```

### Tasks

1. Using a 'while loop', tell your computer to log the numbers from ten to one.
2. Log every 3rd number from 3 to 22 using a 'for loop'.
3. Try to log your favourite food on the console. (use your `favouriteFood` array in the previous step.)

