# javascript note

## Concept, Variable and Datatype

1. **Concept**:
JavaScript is a multi-paradigm, dynamic language with types and operators, standard built-in objects, and methods. Its syntax is based on the Java and C languages — many structures from those languages apply to JavaScript as well.

2. **Variable**:
Variables in JavaScript are declared using one of three keywords: let, const, or var.
let allows you to declare block-level variables. The declared variable is available from the block it is enclosed in.
**let** allows you to declare block-level variables. The declared variable is available from the block it is enclosed in.
```
Example:
let a;
let name = "Simon";

// myLetVariable is *not* visible out here

for (let myLetVariable = 0; myLetVariable < 5; myLetVariable++) {
  // myLetVariable is only visible in here
}
```
**const** allows you to declare variables whose values are never intended to change. The variable is available from the block it is declared in.
```
Example:
const Pi = 3.14; // Declare variable Pi
console.log(Pi); // 3.14
```
**var** declarations can have surprising behaviors (for example, they are not block-scoped), and they are discouraged in modern JavaScript code.

3. **Data types**:

JavaScript programs manipulate values, and those values all belong to a type. JavaScript offers seven primitive types:
**Number**: used for all number values (integer and floating point) except for very big integers.
```
Example:
console.log(3 / 2); // 1.5, not 1
```
**BigInt**: used for arbitrarily large integers.
```
Example:
console.log(-3n / 2n); // -1n
```
**String**: used to store text.
```
Example:
console.log("Hello, world");
console.log("你好，世界！"); // Nearly all Unicode characters can be written literally in string literals
```
**Boolean**: true and false — usually used for conditional logic.
avaScript has a Boolean type, with possible values true and false — both of which are keywords. Any value can be converted to a boolean according to the following rules:

false, 0, empty strings (""), NaN, null, and undefined all become false.
All other values become true.
```
Example:
Boolean(""); // false
Boolean(234); // true
```
**Symbol**: used for creating unique identifiers that won't collide.
```
Example:
const NAME = Symbol()
const person = {
  [NAME]: 'Flavio'
}

person[NAME] //'Flavio'

const RUN = Symbol()
person[RUN] = () => 'Person is running'
console.log(person[RUN]()) //'Person is running'
```
**Undefined**: indicating that a variable has not been assigned a value.
```
Example:
let x;
if (x === undefined) {
  text = "x is undefined";
} else {
  text = "x is defined";
}
```
**Null**: The null value represents the intentional absence of any object value.
```
Example:
typeof null          // "object" (not "null" for legacy reasons)
typeof undefined     // "undefined"
null === undefined   // false
null  == undefined   // true
null === null        // true
null  == null        // true
!null                // true
isNaN(1 + null)      // false
isNaN(1 + undefined) // true
```

