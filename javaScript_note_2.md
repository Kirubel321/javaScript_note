# javascript
## Conditional statement and loops

1. **Conditional statement**

JavaScript has a similar set of control structures to other languages in the C family. Conditional statements are supported by if and else
```
Example:
let name = "kittens";
if (name === "puppies") {
  name += " woof";
} else if (name === "kittens") {
  name += " meow";
} else {
  name += "!";
}
name === "kittens meow";
```
2. **loops**
JavaScript has while loops and do...while loops. The first is good for basic looping; the second is for loops where you wish to ensure that the body of the loop is executed at least once:
```
Examle:
while (true) {
  // an infinite loop!
}

let input;
do {
  input = get_input();
} while (inputIsNotValid(input));

```
JavaScript also contains two other prominent for loops: for...of, which iterates over iterables, most notably arrays, and for...in, which visits all enumerable properties of an object.
```
Example:
for (const value of array) {
  // do something with value
}

for (const property in object) {
  // do something with object property
}
```
The switch statement can be used for multiple branches based on equality checking.
```
Example:
switch (action) {
  case "draw":
    drawIt();
    break;
  case "eat":
    eatIt();
    break;
  default:
    doNothing();
}
```
