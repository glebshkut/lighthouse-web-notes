# Gleb Shkut's Notes

## Summary 

This repository contains all of the notes taken by Gleb Shkut for the Lighthouse Labs Web Development Bootcamp.

taken by [Gleb](https://github.com/JoelCodes) for the [Lighthouse Labs](https://www.lighthouselabs.ca/)

## [Week 1](/Week_1)
  * [Day 1](/Week_1/Day_1)
    - use `eslint [file]` for every javascript code
  * [Day 2](/Week_1/Day_2)
    - use `console.log("arg:", arg)` every time for verify every part of the code
    - create plan without any code syntax (// in commands) and then create code
  * [Day 3](/Week_1/Day_3)
    - `object[key(as a variable)]`; `object ["name"(as a string)]`; `object.name` (as a string, but without double quotes)
    - `this.` is calling this object
    - Метод `Object.keys()` возвращает массив из собственных перечисляемых свойств переданного объекта, в том же порядке, в котором они бы обходились циклом `for...in`
    - Create separate functions as often as possible
    - <b> Don't forget to add .length to simple for loop</b>
  * [Day 4](/Week_1/Day_4)
    - Callback function - function `func` pushed into another function `function callIt = func => {}` as an argument and then was called, by using () to it`func()`
    - Anonymous function - callback function, which is not gonna be declared anywhere, just passed in the func itself `findWaldo(["Alice", "Bob", "Waldo", "Winston"], function(index) {console.log("Waldo is located at:", index);});`
    - <b> `func` which we are passing to our `function` as a parameter is the same as our `action` variable inside `function` function </b>
    - `.filter` return element of array if callback function returns true, ie: `const evens = arrayOfNumbers.filter(function(num) {return num % 2 === 0;});`
    - `numbers.sort((a,b) => a - b)` function is placing `b` first, in case `a - b < 0`
    - closure functions - когда функцию(1) (вызванную) присваивают другой функции(2), и вызывают эту функцию(2), то она должна вернуть функцию, передав ей параметр, и потом та функция уже вернет результат <b> Пробуй представлять фyнкцию в другом виде - к примеру: анонимную в виде обычной, в виде референса </b>
   * [Day 5](/Week_1/Day_5)
     - `this.` is used to get access to current object property and use it for function inside this objects for example..
     - `Object.assign(obj[key], value)` - assign a value in the object
     - `recursion` is when you're doing almost infinitive function: ```function sumToOne(n) {
        if (n === 1) {
         return 1;
        }
        return n + sumToOne(n-1);
        }
       console.log(sumToOne(4));```
     - explain your code to the animated duck, while doing this u can find the solution
     - Before you call yourself stuck, ask yourself the following questions:

`Have I...

...pseudo-coded the solution?

...googled the error message I am getting?

...actually READ the error message?

...double-checked my syntax?

...linted my code?

...pair programmed or gotten a peer to code review?

...rubber-ducked the problem?`
 * [Day 6](/Week_1/Day_6)
     - `npm install mocha chai --save-dev` is used to create mocha and chai for unit testing
## [Week 2](/Week_2)
  * [Day 1](/Week_2/Day_1)
    - `module.exports.myFunc = myFunc;` - can create several functions by using keys. or as an array or object
    - `const myFunc = require('./myFunc');`
    - `.gitignore` for ignoring some files and not sending them ig git repository
    - `const assert = require('chai').assert`
  * [Day_2](/Week_2/Day_2)
    - `process.stdout.write` the same as console.log, but without a new line
    - `setTimeout(() => {console.log(word)}, time);` - timer for some amount of time
    - ![image](https://user-images.githubusercontent.com/56300084/149991170-64342208-ecf5-4487-8bc6-a17e43b59b7c.png)
    - The `on` function is a very common method name for registering callbacks to handle events.
```cjs
const readline = require('readline');

const rl = readline.createInterface({
  input: process.stdin,
  output: process.stdout
});

rl.question('What do you think of Node.js? ', (answer) => {
  console.log(`Thank you for your valuable feedback: ${answer}`);

  rl.close();
});
```
- <br>functions are waiting until other functions will finish their work</br>
* [Day_3](/Week_2/Day_2)
  - ```cjs if (key === '\u0077') {
    client.write("Move: up"); // w
    // process.exit();
  - ```server.on('connection', (client) => {});```
* [Day_5](/Week_2/Day_5)
   - `.bind(obj)` is used if function was called out of its scope and bind will simulate the required object
   - `class Person` - creates a class
   - `class Student extends Person` - creates inhanced class
   - `super.method()` - uses method of super class
   - `get name() {}` - getter of the name
   - `set name(name) {}` - setter of the name
* [Day_1](/Week_3/Day_1)
   - `res.render('filename', templateObject)` renders an html format using variables from template object
* [Day_2](/Week_3/Day_2)
   - `res.redirect("url")` - redirects to url
   - `res.cookie('username', req.body.username)` - creates username cookie using parameters from request body
   - `req.cookies['username']` - looking for a particular cookie
   - use `<form class='form-inline' method="post" action="/login"></form>` to make a form inline 
*** Week 3 ***
* [Day_1] (/Week_4/Day_1) 
```.parent{
  display: flex;
  flex-direction: column;
}
```
- `justify-content:` - on main axis
- `align-items:` - on cross axis
- `order`, which controls the order elements appear in without changing your HTML (its default value is 0)
- `flex-grow`, dictates how much space a flex item should take up
- FLEX-direction:
- `column, column-reverse`
- `row, row-reverse`
- JUSTIFY-content:
- `flex-start`
- `flex-end`
- `center`
- `space-between`
- `space-evenly`
- `space-around`
- ALIGN-items:
- `stretch`
- `flex-start`
- `flex-end`
- `center`
- FLEX-wrap:
- `flex-wrap: nowrap;`
- `flex-wrap: wrap;`
- `flex-wrap: wrap-reverse;`
- ALIGN-content:
- `stretch`
- `flex-start`
- `flex-end`
- `center`
- `space-between`
- `space-around`
- ALIGN-self:
- `flex-start`
- `flex-end`
- `center`
- `stretch`
- `baseline`
- `FLEX-grow:` - increases amount of space one child takes
- `FLEX-shrink` - as value bigger, as smalled child becomes

Day 3
- `div > span` - accesing direct child


REACT NOTES:
React rules:
1. All tags must be closed. There are two ways to close a tag.

```Use two tags (an open tag and a close tag - as with <div>...</div> below).
Use one self-closing tag (as with <Album /> below).
2. A child tag must close before its parent. We are creating a tree structure. So the last one to open is the next one to close.
3. All JSX expressions must result in one root level element. A function can only return one value. A component is defined using a JavaScript function so the same rules apply.
4. No HTML comments.
```

React listens for 3 types of events: onClick, onChange, and onSubmit


GITHUB tips:
- git commit -am "comment" <= same as git add. and then git commit -m
- git revert commit_id <= goes back to the previous commit
- git stash (save *id*) - save changes for later
- git stash pop - for one
- git stach list - list of stashes
- git stash apply *index* - for applying specific one
- git branch -M main - change name of master branch
- git checkout - - go to the previous branch
