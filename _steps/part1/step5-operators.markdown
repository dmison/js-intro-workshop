---
layout: step
number: 5
part: 1
title: Arithmetic Operators
permalink: step5/

#keywords:
#  - term:
#    define:

---

All programming languages have constructs called *operators*. An operator is a character that represents an action, or sometimes a relationship.

You're already familiar with operators from when you learned maths: `+` is an operator that represents the action of *addition*. Operators in programming work the same way.

There are lots of different kinds of operator. For example, you've already used the assignment operator, `=`, to assign a value to your variable in the last step. For this step, we're going to start with *arithmetical* operators, since you already understand how most of them work in the real world.

## Arithmetic Operators

JavaScript includes several standard arithmetical operators (`+`, `-`, `/`, `*`) that you can use to do maths with your numbers.

```javascript
var sumOfNumbers = 1 + 3;
alert(sumOfNumbers);
```

This will pop-up an alert box with the number 4.

Because we're working with numbers here, we don't put quotes around our values, `1` and `3`.

You can use these operators with literal values like numbers or with variables.

```javascript
var first = 10;
var second = 15;
var total = first + second;
alert(total);
```

### Common Arithmetic Operators

There are ten different arthmetic operators in JavaScript.

You can read all about them [here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Arithmetic_Operators
), but the ones you will use most of the time are:

* `+` Addition.  Pretty straight forward.  
    ```javascript
var x = 23 + 2;
    ```
* `-` Subtraction. What you might expect.
    ```javascript
var remainingHP = currentHP - damage;
    ```
* `/`  Division. A forward slash gets used for division.  Think of it like the horizontal line in a fraction.  
    ```javascript
var boxesRequired = numberOfEggs/12;
    ```
* `*`  Multiplication. Multiplication uses an asterisk.
    ```javascript
var boxArea = boxHeight * boxWidth; 
    ```
* `%`  Remainder (AKA Modulus). Not a percentage. It gives you the remainder of a division.  
    ```javascript
var leftOverEggs = numberOfEggs % eggsPerBox;
    ```


#### Increment and Decrement

There are two common operators that operate differently than the others: `++` and `--`.  

These are the increment and decrement operators and unlike most operators they only require a single variable, and they change that variable.

`++` makes a value go up by one.

`--` makes a value go down by one.

```javascript
numberOfAttendees = 20;

// when a new person signs up
numberOfAttendees++;
alert(numberOfAttendees);

//when someone cancels
numberOfAttendees--;
alert(numberOfAttendees);
```

You can only use `++` and `--` on variables.

You'll see more examples of this when we talk about loops later on.

### Why `*` and `/` ?

There are no proper multiplication or division symbols on our keyboards or in any of our programming languages. 

Isn't that weird?  Why is that?

Well, early mechanical typewriters didn't need them so they didn't waste the keys.  They were just typing on paper for people to read, so it only had to look right.  For multiplication we just used `x` or `X`.  For division, we typed a `-`, then moved back one character and typed a `:` over the top of it.  Clever.  Some more expensive typewriters did include extra symbols like divide and multiply but they never reached the same level of popularity as the much cheaper and more reliable models without them.  And more people bought typewriters to write novels and newspaper articles than mathematics papers.

This limitation carried over into the first computer keyboards because of the resource constraints on those machines.  However computers are really picky and unlike a person, they can't easily tell when `x` means multiply and when it means the letter `x`.  And you couldn't type over characters like on paper.  So engineers improvised and picked characters that wouldn't be confusing to the computer and kind of looked right to people, `*` & `/`.  

Fast forward almost a hundred years and we are still using the same system today.


## Operators, strings and concatenation.

Most arithmetic operators don't work on Strings.  For example you can't multiply them or divide them.  There is one exception to this, and that is the addition operator.  When you "add" strings it makes a new string with the other ones joined together.  

This is called **concatenating** them.

```javascript
var firstName = "Diana";
var lastName = "Prince";

var wholeName = firstName + " " + lastName;
alert(wholeName);
```



## Tasks
1. Create 3 variables:
 * 1st variable named ten with value 10 inside
 * 2nd variable named three with value 3
 * 3rd variable named multipleOfNumbers that will be equal to 1st variable multiplied by the 2nd variable.
2. As a result, display the value of multipleOfNumbers.
