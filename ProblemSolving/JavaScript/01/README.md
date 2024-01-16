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



1. **setSeconds(seconds)**
   - Sets the seconds of a `Date` object.
   ```javascript
   const currentDate = new Date();
   currentDate.setSeconds(30);
   console.log(currentDate.getSeconds()); // Output: 30
   ```

2. **setMinutes(minutes)**
   - Sets the minutes of a `Date` object.
   ```javascript
   const currentDate = new Date();
   currentDate.setMinutes(45);
   console.log(currentDate.getMinutes()); // Output: 45
   ```

3. **setHours(hours)**
   - Sets the hours of a `Date` object.
   ```javascript
   const currentDate = new Date();
   currentDate.setHours(12);
   console.log(currentDate.getHours()); // Output: 12
   ```

4. **setDate(day)**
   - Sets the day of the month of a `Date` object.
   ```javascript
   const currentDate = new Date();
   currentDate.setDate(15);
   console.log(currentDate.getDate()); // Output: 15
   ```

5. **setMonth(month)**
   - Sets the month of a `Date` object (0 to 11, where 0 is January and 11 is December).
   ```javascript
   const currentDate = new Date();
   currentDate.setMonth(6); // Sets the month to July
   console.log(currentDate.getMonth()); // Output: 6
   ```

6. **setFullYear(year)**
   - Sets the full year of a `Date` object.
   ```javascript
   const currentDate = new Date();
   currentDate.setFullYear(2023);
   console.log(currentDate.getFullYear()); // Output: 2023
   ```

These methods modify the date and time components of a `Date` object in place. Always remember that months are zero-indexed (0 is January, 1 is February, and so on), and days are one-indexed (1 to 31).

