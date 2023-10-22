# Javascript-Fundamentals topic 3



## Topic 3: Mastering the For Loop

**For Loops**: In JavaScript, a `for` loop is used to repeat a block of code as long as a specified condition is true.

**When to Use**: In our Shoe Selling e-commerce website, you might use a `for` loop to display a list of available shoe sizes, calculate discounts for multiple items, or validate a batch of user inputs.

**Use Case in Websites**: For loops are essential for iterating over arrays, objects, or any set of data. They are commonly used for tasks like populating dropdowns, generating tables, or applying the same operation to multiple elements.

### Examples

#### Example 1: Basic for Loop to Display Numbers

```javascript
// Example 1: Basic for loop to display numbers
for (let i = 1; i <= 5; i++) {
  console.log(i);
}
// Output:
// 1
// 2
// 3
// 4
// 5
```

#### Example 2: For Loop to Display Available Sizes

```javascript
// Example 2: For loop to display available shoe sizes
let availableSizes = [6, 7, 8, 9, 10];
for (let i = 0; i < availableSizes.length; i++) {
  console.log(`Available size: ${availableSizes[i]}`);
}
// Output:
// "Available size: 6"
// "Available size: 7"
// "Available size: 8"
// "Available size: 9"
// "Available size: 10"
```

#### Example 3: For Loop to Calculate Total Price

```javascript
// Example 3: For loop to calculate total price of items in cart
let cart = [120, 80, 200];
let total = 0;
for (let i = 0; i < cart.length; i++) {
  total += cart[i];
}
console.log(`Total price: $${total}`);
// Output: "Total price: $400"
```

### Common Use Cases for For Loops

1. **Iterating Over Arrays**:

   ```javascript
   // Example: Iterating over an array of product names
   let products = ["Sneakers", "Boots", "Sandals", "Heels"];

   console.log("Available Products:");
   for (let i = 0; i < products.length; i++) {
     console.log(`- ${products[i]}`);
   }
   ```

   In this example, we iterate over an array of product names and display them.

2. **Generating Sequences**:

   ```javascript
   // Example: Generating a sequence of even numbers
   console.log("Even Numbers:");
   for (let i = 2; i <= 10; i += 2) {
     console.log(i);
   }
   ```

   Here, we use a for loop to generate a sequence of even numbers.

3. **Accumulating Values**:

   ```javascript
   // Example: Calculating the total quantity in a shopping cart
   let cart = [3, 2, 4, 1, 2];

   let totalQuantity = 0;
   for (let i = 0; i < cart.length; i++) {
     totalQuantity += cart[i];
   }

   console.log(`Total Quantity in Cart: ${totalQuantity}`);
   ```

   This example calculates the total quantity of items in a shopping cart.

4. **Data Validation**:

   ```javascript
   // Example: Validating user input for product ratings
   let ratings = [4, 5, 2, 3, 6];
   let validInput = true;

   for (let i = 0; i < ratings.length; i++) {
     if (ratings[i] < 1 || ratings[i] > 5) {
       validInput = false;
       break;
     }
   }

   if (validInput) {
     console.log("All ratings are valid.");
   } else {
     console.log("Invalid rating detected.");
   }
   ```

   In this example, we validate user input for product ratings and check if they fall within a valid range.

### Exercises

1. **Exercise 3.1: Basic For Loop (Beginner, 5 mins)**  
   - **Objective**: Understand how to use a basic `for` loop.  
   - **Instructions**: Use a `for` loop to display numbers from 1 to 5.  
   - **Desired Output**:  
     ```javascript
     // 1
     // 2
     // 3
     // 4
     // 5
     ```

2. **Exercise 3.2: Looping Through an Array (Intermediate, 10 mins)**  
   - **Objective**: Understand how to loop through an array.  
   - **Instructions**: Use a `for` loop to display available shoe sizes.  
   - **Desired Output**:  
     ```javascript
     // Available size: 6
     // Available size: 7
     // Available size: 8
     // Available size: 9
     // Available size: 10
     ```

3. **Exercise 3.3: Calculating Total Price (Advanced, 15 mins)**  
   - **Objective**: Understand how to use a `for` loop for calculations.  
   - **Instructions**: Use a `for` loop to calculate the total price of items in a cart.  
   - **Desired Output**:  
     ```javascript
     // Total price: $400
     ```

### Solutions with Explanations

#### Exercise 3.1 Solution

```javascript
// Exercise 3.1 Solution
// Using a basic for loop
for (let i = 1; i <= 5; i++) {
  console.log(i);
}
// Here, we declare a variable 'i' and initialize it with 1. The loop will continue as long as 'i' is less than or equal to 5. 
// Each time the loop iterates, 'i' is incremented by 1, and its value is logged to the console.
```

#### Exercise 3.2 Solution

```javascript
// Exercise 3.2 Solution
// Looping through an array
let availableSizes = [6, 7, 8, 9, 10];
for (let i = 0; i < availableSizes.length; i++) {
  console.log(`Available size: ${availableSizes[i]}`);
}
// This solution uses a for loop to iterate through the 'availableSizes' array and display each size.
```

#### Exercise 3.3 Solution

```javascript
// Exercise 3.3 Solution
// Calculating total price with a for loop
let cart = [120, 80, 200];
let total = 0;
for

 (let i = 0; i < cart.length; i++) {
  total += cart[i];
}
console.log(`Total price: $${total}`);
// This solution calculates the total price of items in the 'cart' array by using a for loop to iterate through the items and accumulate their values.
```

---

Feel free to review this topic, and let me know if you'd like to move on to the next topic, "Exploring the While Loop." 📖
