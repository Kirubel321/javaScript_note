# javascript_class

## javaScript

1. **Concept**:
JavaScript is a multi-paradigm, dynamic language with types and operators, standard built-in objects, and methods. Its syntax is based on the Java and C languages — many structures from those languages apply to JavaScript as well.

2. **Variable**:
Variables in JavaScript are declared using one of three keywords: let, const, or var.
let allows you to declare block-level variables. The declared variable is available from the block it is enclosed in.
* let allows you to declare block-level variables. The declared variable is available from the block it is enclosed in.
```
Example:
let a;
let name = "Simon";

// myLetVariable is *not* visible out here

for (let myLetVariable = 0; myLetVariable < 5; myLetVariable++) {
  // myLetVariable is only visible in here
}
```
* const allows you to declare variables whose values are never intended to change. The variable is available from the block it is declared in.
```
Example:
const Pi = 3.14; // Declare variable Pi
console.log(Pi); // 3.14
```
* var declarations can have surprising behaviors (for example, they are not block-scoped), and they are discouraged in modern JavaScript code.


