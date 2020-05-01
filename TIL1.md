# Today I learned  1
---
## JavaScript
Only put simple scripts on html and the more complex files on separate folders.
Because it speed up the browser to put downloaded scripts in cache and use in diferent pages
hyphens '-' aren't allowed in variables
Backticks are “extended functionality” quotes. They allow us to embed variables and expressions into a string by wrapping them in ${…}, for example:
```javascript
let name = "John";
// embed a variable
alert( `Hello, ${name}!` ); // Hello, John!
```

## Change string to Boolean

```javascript
let value = true;
alert(typeof value); // boolean

value = String(value); // now value is a string "true"
alert(typeof value); // string
```

## Numeric Conversion

```javascript
alert( "6" / "2" ); // 3, strings are converted to numbers
```

```javascript
let str = "123";
alert(typeof str); // string

let num = Number(str); // becomes a number 123

alert(typeof num); // number
```

```javascript
let age = Number("an arbitrary string instead of a number");

alert(age); // NaN, conversion failed
```

## Boolean Conversion

```javascript
alert( Boolean(1) ); // true
alert( Boolean(0) ); // false

alert( Boolean("hello") ); // true
alert( Boolean("") ); // false
```

```javascript
alert( Boolean("0") ); // true
alert( Boolean(" ") ); // spaces, also true (any non-empty string is true)
```

## Remainder %

```javascript
alert( 5 % 2 ); // 1 is a remainder of 5 divided by 2
alert( 8 % 3 ); // 2 is a remainder of 8 divided by 3
alert( 6 % 3 ); // 0 is a remainder of 6 divided by 3
```

## Exponenciação **

```javascript
alert( 2 ** 2 ); // 4  (2 * 2)
alert( 2 ** 3 ); // 8  (2 * 2 * 2)
alert( 2 ** 4 ); // 16 (2 * 2 * 2 * 2)
```

## Incremento / decremento

Increasing or decreasing a number by one is among the most common numerical operations.
So, there are special operators for it:

```javascript
let counter = 2;
counter++;        // works the same as counter = counter + 1, but is shorter
alert( counter ); // 3
```

```javascript
let counter = 2;
counter--;        // works the same as counter = counter - 1, but is shorter
alert( counter ); // 1
```

```javascript
let counter = 1;
let a = ++counter; // (*)

alert(a); // 2
```

```javascript
let counter = 1;
let a = counter++; // (*) changed ++counter to counter++

alert(a); // 1
```