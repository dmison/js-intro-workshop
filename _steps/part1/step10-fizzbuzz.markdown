---
layout: step
number: 10
part: 1
title: "Exercise: FizzBuzz"
permalink: step10/

---
OK, time for an exercise: FizzBuzz.  :tada:

FizzBuzz is simple counting game for teaching division. It got a small amount of fame in the programming community a few years ago when it was used as an example of an screening question for job interviews.  

> Players generally sit in a circle. The player designated to go first says the number "1", and each player counts one number in turn. However, any number divisible by three is replaced by the word fizz and any divisible by five by the word buzz. Numbers divisible by both become fizz buzz. A player who hesitates or makes a mistake is eliminated from the game.

You can read more about it on [Wikipedia](https://en.wikipedia.org/wiki/Fizz_buzz) if you want.

For our purposes FizzBuzz will work like this:

1. You need to display a list of the numbers from 1 to 50.
2. If a number is a multiple of three, display 'Fizz' instead.
3. If it's a multiple of 5, display 'Buzz' instead.
4. If it's a multiple of 3 and 5, print 'FizzBuzz' instead.

So for the numbers 1 to 15 the output would look like:

```
1
2
Fizz
4
Buzz
Fizz
7
8
Fizz
Buzz
11
Fizz
13
14
FizzBuzz
```

Give it a try, don't forget to ask for help if you get stuck.

#### Hints:

1. Use `console.log()` to display each number or Fizz/Buzz.
2. To display a list of numbers you might want to use a loop
3. Is there an arithmetic operator that would make it easier to work out if one number is a multiple of another?
4. If it seems like a lot, just try getting the first step done.  Then add the second one, and so on.

If you get part way through and think of a better way of doing it, don't delete what you've done.  Just comment it out and start again under it.  This way you will be able to refer to your original if you need to.  My code is always a mess of commented out attempts before I figure out the answer and then I delete all the old comments.

```javascript
for( var i= 0; i < 50; i++){
    if(i % 15 == 0){
        console.log("FizzBuzz");
    }
    else if(i % 3 == 0){
        console.log("Fizz")
    }
    else if(i % 5 == 0){
        console.log("Buzz");
    }
    else {
        console.log(i);
    }
}
```
{: .solution }


There is more than one solution to any problem of course.  This is just one way.  How might you do it using only one `console.log()`? (Hint: by joining strings.) 