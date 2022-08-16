# dom-filesystem
Use the Node.js fs API inside Javascript and store the data inside the DOM, good for creating quines.

## Installing
npm add dom-filesystem
yarn add dom-filesystem

## Using
```javascript
let fs = require("dom-filesystem")(document)

function async main() {
  fs.writeFileSync( "/hello-world.txt", "hello-world")
  let result = fs.readFileSync("/hello-world.txt")
  console.log( result )
}
```
