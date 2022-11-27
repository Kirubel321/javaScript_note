# javaScript
## Function,Arrays and DOM Manipulation

1. **Function**:
A JavaScript function can take 0 or more parameters. The function body can contain as many statements as you like and can declare its own variables which are local to that function. The return statement can be used to return a value at any time, terminating the function. If no return statement is used (or an empty return with no value), JavaScript returns undefined.
```
Example:
function add(x, y) {
  const total = x + y;
  return total;
}
```
2. **Arrays**:
Arrays in JavaScript are actually a special type of object. They work very much like regular objects (numerical properties can naturally be accessed only using [] syntax) but they have one magic property called length. This is always one more than the highest index in the array.
```
Example:
Arrays are usually created with array literals:
const a = ["dog", "cat", "hen"];
a.length; // 3

```
3. **DOM Manipulation**
The Document Object Model (DOM) is the data representation of the objects that comprise the structure and content of a document on the web.
The Document Object Model (DOM) is a programming interface for web documents. It represents the page so that programs can change the document structure, style, and content. The DOM represents the document as nodes and objects; that way, programming languages can interact with the page.
```
Example:
The DOM specifies that the querySelectorAll method in this code snippet must return a list of all the <p> elements in the document:
const paragraphs = document.querySelectorAll("p");
// paragraphs[0] is the first <p> element
// paragraphs[1] is the second <p> element, etc.
alert(paragraphs[0].nodeName);
The following function creates a new <h1> element, adds text to that element, and then adds it to the tree for the document:
<html lang="en">
  <head>
    <script>
      // run this function when the document is loaded
      window.onload = () => {
        // create a couple of elements in an otherwise empty HTML page
        const heading = document.createElement("h1");
        const headingText = document.createTextNode("Big Head!");
        heading.appendChild(headingText);
        document.body.appendChild(heading);
      };
    </script>
  </head>
  <body></body>
</html>
```
