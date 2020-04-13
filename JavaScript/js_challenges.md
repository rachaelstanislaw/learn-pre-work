## JavaScript Challenges

**1. JS Math!**

_Developer notes: will need an IDE of sorts or chrome console for this one_

Practice with this arithmetic:
- Multiply 77 times 38 --> 2926
- Add 6.7 and -40 --> -33.3
- Subtract 2 from 21 --> 19
- Divide 99 by 3 --> 33

**2. Variable Practice**

- Set a variable called `myDog` to equal `Bolt`
- Set another variable to `myCat` to equal `Duchess`
- Set another variable to `myFish` to equal `Bubbles`
- Call `myDog`, `myCat`, and `myFish`
- Reassign `myDog` to equal `Mopsy` and `myFish` to equal `Speedy`
- Call `myDog`, `myCat`, and `myFish`

```javascript
var myDog = "Bolt"
var myCat = "Duchess"
var myFish = "Bubbles

myDog     // "Bolt"
myCat     // "Duchess"
myFish    // "Bubbles"

myDog = "Mopsy
myFish = "Speedy"

myDog     // "Mopsy"
myCat     // "Duchess"
myFish    // "Speedy"
```

**3. Understaning Loops/Iteration**

- The first loop should return: `0, 1, 2, 3, 4`
- The second loop should return: `10, 9, 8, 7, 6, 5, 4, 3, 2, 1`
- Fill in this loop that will only return the number 10. Hint: you will need to incorporate an `if` conditional! What will be the final return?

```javascript
var numbers = [7, 8, 10, 3, 10, 5, 66, 10, 2]

for(let i = 0; i < numbers.length; i__) {   // 1. ++
  if(______[i] === 10) {                    // 2. numbers
    console.log(numbers__);                 // 3. [i]
  }                                         // 4. final return is: 10 10 10
}
```

**4. Function Practice**

- Write a function called `niceWork` that returns `"High five!"` every time it is invoked. Don't forget to add the function call at the end.
```javascript
niceWork = () => {
  console.log("High five!")
}

niceWork()
```

- Fill in the blanks for this function. We want to return the second name in the array. What will be the final results?
```javascript
var names1 = ["Stacy", "Jenna", "Melanie", "Beth", "Michelle"]
var names2 = ["Jose", "Rodrigo", "Sean", "Josh", "Grant"]

secondName = (array) => {
  console.log(_____[__]);     // 1. array
}                             // 2. 1

secondName(names1)            // 3. "Jenna"
secondName(names2)            // 4. "Rodrigo"
```
- Write a function called `wildWest` that accepts any number greater than 0 as an argument. The function will return `"Darn tootin'!"` if the argument is 1, `"Get yer ice cold sarsaparilla!"` if the argument is 2, or `"This town aint big enough for the both of us"` if the argument is anything else. Hint: you will need `if else` conditionals in your function! Feel free to copy and paste the return values. Don't forget to add the function call at the end.
```javascript
wildWest = (num) => {
  if(num === 1) {
    console.log("Darn tootin'!");
  } else if(num === 2) {
    console.log("Get yer ice cold sarsaparilla!");
  } else {
    console.log("This town aint big enough for the both of us");
  }
}

wildWest(1)     // "Darn tootin'!"
wildWest(2)     // "Get yer ice cold sarsaparilla!"
wildWest(50)    // "This town aint big enough for the both of us"
```

<a href="https://github.com/rachaelstanislaw/learn-pre-work/blob/master/JavaScript/js_lectures.md">Go back to lectures</a>

<a href="https://github.com/rachaelstanislaw/learn-pre-work">Back to Table of Contents</a>
