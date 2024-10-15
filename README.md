# js

JavaScript provides a rich set of array functions to manipulate and interact with arrays effectively. Below are some commonly used **array functions** along with examples:

### 1. **`map()`**
Transforms each element in an array and returns a new array.
```javascript
const numbers = [1, 2, 3, 4];
const doubled = numbers.map(num => num * 2); 
console.log(doubled); // [2, 4, 6, 8]
```

### 2. **`filter()`**
Creates a new array with all elements that pass the test implemented by a provided function.
```javascript
const numbers = [1, 2, 3, 4];
const evenNumbers = numbers.filter(num => num % 2 === 0);
console.log(evenNumbers); // [2, 4]
```

### 3. **`reduce()`**
Applies a function against an accumulator and each element to reduce the array to a single value.
```javascript
const numbers = [1, 2, 3, 4];
const sum = numbers.reduce((accumulator, current) => accumulator + current, 0);
console.log(sum); // 10
```

### 4. **`forEach()`**
Executes a provided function once for each array element (no return value).
```javascript
const numbers = [1, 2, 3];
numbers.forEach(num => console.log(num * 2));
// Output: 2, 4, 6
```

### 5. **`find()`**
Returns the value of the first element that satisfies the provided testing function.
```javascript
const numbers = [1, 2, 3, 4];
const found = numbers.find(num => num > 2);
console.log(found); // 3
```

### 6. **`findIndex()`**
Returns the index of the first element that satisfies the provided testing function.
```javascript
const numbers = [1, 2, 3, 4];
const index = numbers.findIndex(num => num > 2);
console.log(index); // 2
```

### 7. **`some()`**
Checks if at least one element in the array passes the test implemented by the provided function.
```javascript
const numbers = [1, 2, 3, 4];
const hasEven = numbers.some(num => num % 2 === 0);
console.log(hasEven); // true
```

### 8. **`every()`**
Checks if all elements in the array pass the test implemented by the provided function.
```javascript
const numbers = [1, 2, 3, 4];
const allEven = numbers.every(num => num % 2 === 0);
console.log(allEven); // false
```

### 9. **`includes()`**
Determines whether an array contains a certain element.
```javascript
const fruits = ['apple', 'banana', 'orange'];
const hasBanana = fruits.includes('banana');
console.log(hasBanana); // true
```

### 10. **`sort()`**
Sorts the elements of an array **in place** and returns the sorted array.
```javascript
const numbers = [4, 1, 3, 2];
numbers.sort((a, b) => a - b); // Ascending order
console.log(numbers); // [1, 2, 3, 4]
```

### 11. **`concat()`**
Merges two or more arrays into a new array.
```javascript
const array1 = [1, 2];
const array2 = [3, 4];
const combined = array1.concat(array2);
console.log(combined); // [1, 2, 3, 4]
```

### 12. **`slice()`**
Returns a shallow copy of a portion of an array into a new array (does not modify the original array).
```javascript
const numbers = [1, 2, 3, 4, 5];
const sliced = numbers.slice(1, 4);
console.log(sliced); // [2, 3, 4]
```

### 13. **`splice()`**
Adds/removes elements from an array and returns the removed elements (modifies the original array).
```javascript
const numbers = [1, 2, 3, 4];
const removed = numbers.splice(1, 2); // Removes 2 elements starting at index 1
console.log(numbers); // [1, 4]
console.log(removed); // [2, 3]
```

### 14. **`join()`**
Joins all elements of an array into a string.
```javascript
const elements = ['Fire', 'Wind', 'Earth'];
const joined = elements.join(', ');
console.log(joined); // "Fire, Wind, Earth"
```

### 15. **`reverse()`**
Reverses the array **in place**.
```javascript
const numbers = [1, 2, 3];
numbers.reverse();
console.log(numbers); // [3, 2, 1]
```

### 16. **`push()` and `pop()`**
- `push()` adds one or more elements to the end of an array.
- `pop()` removes the last element from an array.
```javascript
const numbers = [1, 2];
numbers.push(3); // Adds 3
console.log(numbers); // [1, 2, 3]
numbers.pop(); // Removes 3
console.log(numbers); // [1, 2]
```

### 17. **`shift()` and `unshift()`**
- `shift()` removes the first element from an array.
- `unshift()` adds one or more elements to the beginning of an array.
```javascript
const numbers = [2, 3];
numbers.unshift(1); // Adds 1 at the start
console.log(numbers); // [1, 2, 3]
numbers.shift(); // Removes 1
console.log(numbers); // [2, 3]
```

These functions make it easy to work with arrays in JavaScript, providing powerful tools to manipulate, search, and transform data.
