## JavaScript Content

### Module 1: Intro to JavaScript ###
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
  - `==` converts the data values to the same data type before performing comparison through _type coercion_. 
  - `===` does not do any type coercion and returns **true** _only_ if both values and types are identical. For example:
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
- Not: `!` (this should be familiar!), negates the proceeding statement

```javascript
// and
true && false       // false
true && true        // true

// or
true  || false      // true
false || false      // false
  
// not
!true               // false
!false              // true
true != false       // true
true != true        // false
!(true && false)    // true
!(true && false)    // true
```

### Module 2: Variables ###



<a href="https://github.com/rachaelstanislaw/learn-pre-work/blob/master/JavaScript/js_challenges.md">Go to challenges</a>

<a href="https://github.com/rachaelstanislaw/learn-pre-work">Back to Table of Contents</a>
