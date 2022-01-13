# Gleb Shkut's Notes

## Summary 

This repository contains all of the notes taken by Gleb Shkut for the Lighthouse Labs Web Development Bootcamp.

taken by [Gleb](https://github.com/JoelCodes) for the [Lighthouse Labs](https://www.lighthouselabs.ca/)

* [Week 1](/Week_1)
  * [Day 1](/Week_1/Day_1)
    - use `eslint [file]` for every javascript code
  * [Day 2]
    - use `console.log("arg:", arg)` every time for verify every part of the code
    - create plan without any code syntax (// in commands) and then create code
  * [Day 3]
    - `object[key(as a variable)]`; `object ["name"(as a string)]`; `object.name` (as a string, but without double quotes)
    - `this.` is calling this object
    - Метод `Object.keys()` возвращает массив из собственных перечисляемых свойств переданного объекта, в том же порядке, в котором они бы обходились циклом `for...in`
    - Create separate functions as often as possible
    - <b> Don't forget to add .length to simple for loop</b>
  * [Day 4]
    - Callback function - function `func` pushed into another function `function callIt = func => {}` as an argument and then was called, by using () to it`func()`
    - Anonymous function - callback function, which is not gonna be declared anywhere, just passed in the func itself `findWaldo(["Alice", "Bob", "Waldo", "Winston"], function(index) {console.log("Waldo is located at:", index);});`
