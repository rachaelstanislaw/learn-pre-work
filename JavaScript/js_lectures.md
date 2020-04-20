# JavaScript Content

## Module 1: Intro to JavaScript ##
**1. What is JS?**

JavaScript (often shortened to "JS") is a powerful, flexible, and fast programming language. It was created in 1995 so it's old and well documented. Java and JavaScript are not the same language! JavaScript is most commonly used as a client side scripting language. This means that JavaScript code is written into an HTML page and when a user requests an HTML page with JavaScript in it, the script is sent to the browser (chrome) and it's up to the browser to do something with it. If HTML is the skeleton of a program, think of JavaScript as the muscular system! It gives your user something to interact with!

**2. Primitive Data Types**

A _data type_ is an attribute of data which tells the compiler or interpreter how the programmer intends to use the data. There are six primitive data types in JS:

- Number
- String
- Boolean
- Null
- Undefined
- Symbol

In this module, we will focus on number, string, and boolean.

- **Numbers** are exactly that! Numbers! JS numbers can be positive, negative, whole numbers, and floats (a number with fractional value such as 2.5).

We can perform basic math with numbers in JS

Addition: `4 + 100`

Subtraction: `40 - 6`

Multiplication: `76 * 2`

Division: `9 / 3`

- **Strings** are anything wrapped in quotation marks! _All_ of the following examples are strings:

```javascript
"Salt and Pepper Kettle Chips"
"True"
"100"
```

- **Booleans** are the value of either _true_ or _false_.

**3. Comparison Operators**

Coding is going to require a lot of comparisons! We can compare values a couple different ways. 

- Equality operator: `==` or `===`
  - `==` converts the data values to the same data type before performing comparison through _type coercion_. This is an _Abstrct Equality Comparison_
  - `===` does not do any type coercion and returns **true** _only_ if both values and types are identical. This is a _Strict Equality Comparison_. For example:
```javascript
4 == 4        // true
7 == 4        // false
"4" == 4      // true
"4" === 4     // false
"4" !== 4     // true
```

Hey, what was that `!` ?? The `!` above is called a _bang operator_. The bang operator essentially says "String 4 is _not_ equal to number 4" which is true.

**4. Relational Operators**

You can also compare values with Relational Operators: `>`, `<`, `>=`, `<=`

```javascript
// greater than
2 > 0         // true

// less than
4 < 8         // true

// greater than or equal to
0 >= 2        // false

// less than or equal to
-4 <= 0.8     // true
```

**5. Logical Operators**

- And: `&&`, checks if _both_ values meet a certain criteria
- Or: `||`, checks if _at least one_ value meets a certain criteria
- Not: `!` (this should be familiar), negates the proceeding statement

```javascript
// and
4 && 7 > 1          // true
11 && 12 < 6        //false

// or
true  || false      // true
false || false      // false
  
// not
!true               // false
!false              // true
true !== false       // true
true !== true        // false
!(true && false)    // true
!(true && false)    // true
```

## Module 2: Variables ##

JavaScript variables are containers for storing data values. They are re-usable and re-assignable in most cases. Think of a variable as a piece of Tupperware...

My Tupperware is labeled "Lunch." Yesterday, I decided to pack myself a sandwich 

<img src="https://i.ibb.co/10dZSGG/Screen-Shot-2020-04-09-at-5-36-51-PM.png" alt="Screen-Shot-2020-04-09-at-5-36-51-PM" border="0">

When 12 o'clock rolled around and I opened up my Tupperware, a sandwich was inside

<img src="https://i.ibb.co/xS5qrX1/Screen-Shot-2020-04-09-at-5-36-53-PM.png" alt="Screen-Shot-2020-04-09-at-5-36-53-PM" border="0">

Every time I opened up my lunch container throughout the day, I saw a sandwich. It did not change. 

But today I decided I would like tacos for lunch instead of a sandwich. I used my same container labeled "Lunch" and replaced its contents with tacos 

<img src="https://i.ibb.co/6DQMJxB/Screen-Shot-2020-04-09-at-5-36-59-PM.png" alt="Screen-Shot-2020-04-09-at-5-36-59-PM" border="0">

Once again, it's lunchtime. I opened my lunch container to find tacos. There was no need for me to create more dishes and start a new lunch container. I reused the orignial one! I successfully re-assigned my variable!

<img src="https://i.ibb.co/W2wNvmq/Screen-Shot-2020-04-09-at-5-37-00-PM.png" alt="Screen-Shot-2020-04-09-at-5-37-00-PM" border="0">

Let's look at what this looks like in code:

```javascript
var lunch = "sandwich"    // assign a variable using the (keyword "var") + (the name of your variable) + (a single =) + (data)

lunch                     // "sandwich"
lunch                     // "sandwich"
lunch                     // "sandwich"

lunch = "taco"            // reassign variable data with (the name of your variable) + (a single =) + (data)

lunch                     // "taco"
```

So far we have covered `==` and `===` for comparing data. But a single `=` _assigns value_. Also, variable names are **lowercase**!

_Developer notes: small activities after this module_

## Module 3: Conditionals ##

A conditional statement (also called an if/else statement or a decision tree), is a way to tell your program how to behave based on certain circumstances.

- First, we need to declare a condition to be met. We do that by writing `if` immediately followed by a pair of parentheses `()`. We are going to put our condition inside of the parentheses:

```javascript
if(!hungry)
```

- Now we will add a new line to this code that tells our program what to do if the condition is _true_. We do this by adding an _opening curly brace_ `{` before dropping to the next line and adding our behavior. Once we add our desired behavior, we drop down one more line and add a _closing curly brace_ `}`:

```javascript
if(!hungry) {
  "keep coding!"
  }
```
The code above is essentially saying "If _not_ hungry is true, keep coding!"

- So what happens if `!hungry` is false? Let's add a little more logic in the form of an `else` statement. Hence `if/else` statements ;). Again, we open up our curly braces, write what we want our program to do, then close the curly braces on the following line:

```javascript
if(!hungry) {
  "keep coding!"
} else {
  "eat a snack!"
}
```

Right now, our program says `if` _this_ is true, do something. Otherwise, do something _else_. Our `else` statement acts as a catch-all for _any thing_ that doesn't meet the `if` requirement. Let's look at what to do when the choices for our program are not so black and white. We do this by adding an `else if` statement before the `else`:

```javascript
if(hungry) {
  "eat a snack!"
} else if(sleepy) {
  "take a nap!"
} else {
  "keep coding!"
}
```

The `else if` statement has a condition that has to be met in order for the block of code `"take a nap!"` to be run so it's syntax is very similar to that of the `if` statement. You can have as many `else if`'s as you'd like to check for as many conditions as you want! However, there can only be _one_ `if` and _one_ `else`.

## Module 4: Arrays ##

**1. Intro to arrays** 

Until now, we've only dealt with one piece of information at a time: one number, one string, one element on a page. But, often we need to group things together. For example, what if we wanted to have a list of the months of the year? We'd use an array, which is just a list of things grouped together.

Here are a few examples of arrays assigned to variables:

```javascript
var months = ["January", "February", "March", "April", "May"]

var numbers = [17, 15, 14, 3, 5, 10]

var combined = [17, "January", 15, "February", 14, "March", 3, "April", 5, "May", 10]
```

Notice that strings in an array have quotes, but numbers don't need them.

The anatomy of an array consists of the following characteristics:
- Brackets `[ ]` with a comma in between each item
- Value in between each commma
- A hidden _index_ that exists behind each value

In JS, index starts at 0
```javascript
var letters = ["l", "e", "a", "r", "n", " ", "S", "D"]
```
What letter is at index 2? ^^^

**2. Accessing Elements in Arrays**

To access the values stored inside of your array, you will need to name the array you're accessing, followed by the _index_ of the value you want to extract. Here's an example:

```javascript
var names = ["Little Red Riding Hood", "Grandma", "Big Bad Wolf"]

names[2]      // "Big Bad Wolf"
names[0]      // "Little Red Riding Hood"
```

## Module 5: For Loops ##

Quick note: In the following sections we will be referring to something called `console.log()`. The `console.log()` is a function that logs a message to a debugging console for the developer. It's a very common way of testing out and debugging your code. For the following modules, think of it as printing an answer for you!

A for loop _iterates_ (typically through an array). On each iteration of the loop, it will do something to the current index before moving on to the next. If this isn't making sense yet, that's ok! We will practice with iteration a lot, it's just important to become familiar with how looping works ;)

Let's look at the anatomy of a `for loop` :
- Where the count starts. What index of the array should I begin my loop on?
```javascript
for(let i = 0; ...
```
- How many iterations we want the loop to go through. This example says, "Do the loop as long as the current index is less than 5"
```javascript
for(let i = 0; i < 5; ...
```
- What to do after each iteration. This example with `i++` says, "Keep iterating _incrementally_"
```javascript
for(let i = 0; i < 5; i++) ...
```
- The thing you'd like to happen on each iteration
```javascript
for(let i = 0; i < 5; i++) {
  console.log(i)
}
```
What do you think the code above does?

_Developer notes: small check for understanding here_

How about this one?
```javascript
for(let i = 10; i > 0; i--) {
  console.log(i)
}
```
`i--` says, "Keep iterating _decrementally_"

_Developer notes: small check for understanding here_

Great! Loops are often used when you'd like to do something to each element of an array. What if I had an array of numbers and wanted to mulitply all of the numbers by 3? One option is to use a for loop. There are more optimized solutions to this example which we will talk about later in the program.

```javascript
var arrayOfNumbers = [5, 3, 2, 9, 8]
for(let i = 0; i < arrayOfNumbers.length; i++) {
  console.log(arrayOfNumbers[i] * 3)
}
```

- The first iteration of the loop starts at index 0
```javascript
var arrayOfNumbers = [5, 3, 2, 9, 8]
                      ^
                      // At index 0, we console.log() the current value * 3
                      // This prints 15
```
- The second iteration of the loop moves on to index 1
```javascript
var arrayOfNumbers = [5, 3, 2, 9, 8]
                         ^
                         // At index 1, we console.log() the current value * 3
                         // This prints 9
```
- Third iteration moves to index 2
```javascript
var arrayOfNumbers = [5, 3, 2, 9, 8]
                            ^
                            // At index 2, we console.log() the current value * 3
                            // This prints 6
```
- So on an so forth until the end of the array...
- Final result should be `15, 9, 6, 27, 24`

## Module 6: Functions ##

According to W3 Schools, a JavaScript function is a block of code designed to perform a particular task. A JavaScript function is executed when it is _invoked_ by a _function call_. Functions should be written to be as reusable as possible.

Let's take the example from the last module. We had a loop that could iterate through `arrayOfNumbers` and produce the contents multiplied by 3. But what if we wanted to mulitply the elements of ten other arrays by 3? We would have to re-write the loop ten more times to accommodate each array. What a pain! 

But alas! Look to the sky! Is that a bird? Or a plane?? No!! It's a _function_, here to save you from your key-stroke woes!

Functions wrap logic into reusable machines, and they are awesome. Let's take a look at the anatomy of a function:

- The _function declaration_ is the name of the function
```javascript
multByThree ...
```
- The _arguments_ your function will take. Arguments are outside information that the function will need access to in order to run. Here, we are using a variable `array` to represent any array that we would like to give our function access to. We are not hard-coding in a specific array.
```javascript
multByThree = (array) ...
```
- The _fat arrow_ is a concise syntax for writing functions. We will talk more about other ways that you may see functions written, as well as more info on _fat arrows_ or _arrow functions_ in the program. Here, we will write our fat arrow followed by curly braces to emcompass our function logic
```javascript
multByThree = (array) => {
}
```
- All of our logic must fall inside of the function's openging and closing curly braces. We will use the for loop from the previous module. But this time, it will be reusable. See if you can spot the differences!
```javascript
multByThree = (array) => {
  for(let i = 0; i < array.length; i++) {
    console.log(array[i] * 3)
  }
}
```
- Last but certainly not least, we will need to _invoke_ our function. Right now, it's a machine in our code just waiting to be run! We do this by calling the name of the function followed by parentheses. If the function requires an argument (this one does!), the argument will go between the parentheses
```javascript
var arrayOfNumbers1 = [5, 3, 2, 9, 8]   // We have added some arrays that we would like to run through the function
var arrayOfNumbers2 = [4, 10, 6, 3]
var arrayOfNumbers3 = [444, 2.5, 7, -4]

multByThree = (array) => {
  for(let i = 0; i < array.length; i++) {
    console.log(array[i] * 3)
  }
}

multByThree(arrayOfNumbers1)           // Between the (), we write the name of the array we want the function to act on
multByThree(arrayOfNumbers2)           // We are calling the funciton multiple times on multiple arrays
multByThree(arrayOfNumbers3)           // For each array that's passed into the function, we get a different result!
``` 

_Developer notes: Quick function practice!_

Not all functions will require an argument. Here's a simple example:

```javascript
sayHello = () => {
  console.log("Hello there! I'm a computer!")
}

sayHello()
```
This code doesn't need access to outside information to run normally. To invoke the function, we simply call it's name followed by parentheses.

<a href="https://github.com/rachaelstanislaw/learn-pre-work/blob/master/JavaScript/js_challenges.md">Go to challenges</a>

<a href="https://github.com/rachaelstanislaw/learn-pre-work">Back to Table of Contents</a>
