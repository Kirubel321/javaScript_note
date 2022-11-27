#javaScript
## Methods and Events 
1. **Methods**:
JavaScript methods are actions that can be performed on objects.
A JavaScript method is a property containing a function definition.
```
Example:
person.name = function () {
  return this.firstName + " " + this.lastName;
};
```
2. **Events**:
Events are actions or occurrences that happen in the system you are programming, which the system tells you about so your code can react to them.
For example:
* The user selects, clicks, or hovers the cursor over a certain element.
* The user chooses a key on the keyboard.
* The user resizes or closes the browser window.
* A web page finishes loading.
* A form is submitted.
* A video is played, paused, or ends.
* An error occurs.
```
Example:
<button>Change color</button>

const btn = document.querySelector('button');

function random(number) {
  return Math.floor(Math.random() * (number+1));
}

btn.addEventListener('click', () => {
  const rndCol = `rgb(${random(255)}, ${random(255)}, ${random(255)})`;
  document.body.style.backgroundColor = rndCol;
});
```
