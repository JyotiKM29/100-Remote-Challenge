# ⏱️ Clock 

### learning:👩🏻‍💻
- Create Date : using `new Date()` function ,
- can access seconds , minutes and hours using `getSeconds` , `getMinutes` and `getHours`
- For rotating from origin ` transform-origin: 100%`
- what is `setInterval` , `padStart()`


 The `padStart()` method in JavaScript is like adding cushions to the beginning of a string to make it a certain length. It ensures a string reaches a desired length by filling in characters (or repeating them) at the start until the specified length is achieved. This is commonly used to format strings, making sure they have a minimum length for neat and consistent presentation.

 ``` 
 const currentDate = new Date();

const paddedHours = String(currentDate.getHours()).padStart(2, '0');
const paddedMinutes = String(currentDate.getMinutes()).padStart(2, '0');
const paddedSeconds = String(currentDate.getSeconds()).padStart(2, '0');

// Display the padded time
console.log(`Padded Time: ${paddedHours}:${paddedMinutes}:${paddedSeconds}`);

```
output:
```
Padded Time: 02:08:00

```


