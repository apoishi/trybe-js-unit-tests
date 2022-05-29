## About the project
This repository contains the js unit tests project developed while studyng at Trybe. This project is an implementation of various functions using JavaScript and/or unit tests.

## Skills
- Write unit tests using the NodeJS Jest module to verify the correct functioning of the functions;
- Write functions so that they meet already implemented tests;
- Write tests and functions using a test-driven development approach.

## Mandatory requirements

### 1. Implement the `average` function

<details>
  <summary>The average function takes a variable-length array and returns the average of the values ​​received. If the function receives some non-numeric value or an empty array, the value `undefined` must be returned. All results must be rounded to integers. Ex: 4.6 becomes 5; 1.3 becomes 1. The `average.spec.js` file contains the tests for `average` already implemented. Implement the function in the `src/average.js` file so that it meets the proposed tests.</summary><br/>


  **What will be tested:**

  - It will be validated if, when receiving an array of numbers, the `average` function returns the average of its values;
  - It will be validated if, when receiving an array that contains non-numeric values, the `average` function returns `undefined`;
  - It will be validated if, when receiving an empty array, the `average` function returns `undefined`.

</details>


### 2. Implement the test cases for the `numbers` function

<details>
  <summary>The `numbers` function takes a variable-length array and returns `true` if all parameters are of type 'number' and `false` otherwise. This function is already implemented in the `src/numbers.js` file. Write at least four tests for this function to ensure that the implementation of `numbers` is correct.</summary><br/>

  **What will be tested:**

  - It will be validated if in the test of the `numbers` function, the function return is `true` when the array passed by parameter contains only numbers.

</details>


### 3. Implement the `vqv` function

<details>
  <summary>Use template literals to write a function that takes its name and age and returns the paragraph described below:</summary><br/>

  ```javascript
  `Hi, my name is Tunico!
  I'm 30 years old,
  I work at Trybe and I do a lot of programming!
  #VQV!`
  ```

  If the function is called without any parameters, the value `undefined` must be returned. The `vqv.spec.js` file contains the tests for `vqv` already implemented. Implement the function in the `src/vqv.js` file so that it meets the proposed tests.

  **What will be evaluated**

  - It will be validated if `vqv` is a function;
  - It will be validated if the `vqv` function returns string data;
  - It will be validated if the `vqv` function returns the expected phrase when passed parameters of name and age;
  - It will be validated if the `vqv` function, when called without parameter, returns `undefined`.

</details>


### 4. Implement the test cases for the `circle` function

<details>

  <summary>The `circle` function receives the radius of a circle and returns an object containing its information: Radius, Area and Circumference. If no radius is specified, the function returns `undefined`. This function is already implemented in the `src/circle.js` file. Write at least six tests for this function to ensure that the implementation of `circle` is correct.</summary></br>

  **What will be evaluated**

  - It will be validated if in the test of the `circle` function, when receiving a radius, the function return is an object with the correct information (Radius, Area and Circumference).

</details>


### 5. Implement the `createStudent` function

<details>
<summary>The `createStudent` function takes as a parameter a **name**, and returns an object containing two keys:</summary></br>

  1. **name**, containing the name passed as a parameter;
  2. **feedback**, containing a function that returns the phrase 'Jeez good person!' when being called.

  The `createStudent.spec.js` file contains the tests for `createStudent` already implemented. Implement the function in the `src/createStudent.js` file so that it meets the proposed tests.

  **What will be evaluated**

  - It will be validated if the `createStudent` function returns an object that contains two keys: `name`, containing the name passed as a parameter; and `feedback`, containing a function that returns the phrase 'Jeez good person!' when being called.

</details>


### 6. Implement the test cases for the `productDetails` function

<details>
  <summary>The `productDetails` function takes two strings representing product names, and returns an array containing two objects with the details of the respective products:</summary></br>

  ```javascript
  productDetails('Alcohol gel', 'Mask');
  ```

  **Returns:**

  ```js
  [
    {
      name: 'Alcohol gel'
      details: {
        productId: 'Alcohol gel123'
      }
    },
    {
      name: 'Mask'
      details: {
        productId: 'Mask123'
      }
    }
  ]
  ```

  This function is already implemented in the `src/productDetails.js` file. Write at least five tests for this function in the `tests/productDetails.js` file to ensure that the `productDetails` implementation is correct.

  **What will be evaluated**

  - It will be validated if in the test of the `productDetails` function, when receiving two strings, the function return is an array of objects and if each object contains the necessary data.

</details>


### 7. Implement the `calculator` and `arrayGenerator` functions

<details>
  <summary>The `calculator` function takes two integers as a parameter and returns an object with the following braces:</summary></br>
  - sum;
  - multi;
  - div;
  - sub.

  For each key, assign the corresponding operation to its key as a value:
  - `sum:` returns the result of the sum of the two numbers;
  - `mult:` returns the result of multiplying the two numbers;
  - `div:` returns the result of dividing the two numbers;
  - `sub:` returns the result of subtracting the two numbers.

  Division results should always be rounded down.

  Parameters:
  - Two whole numbers.

  Behavior:
  ```javascript
  calculator(1, 2); // { sum: 3, mult: 2, div: 0, sub: -1 }
  ```

  The `arrayGenerator` function converts objects into arrays, of keys, values ​​or both. It must take two parameters:

  - the first parameter must be a string that indicates the type of conversion;
  - the second parameter should be an object similar to the one returned by the calculator function you just developed.

  Parameters:
  - A string indicating the type of conversion;
  - An object in the format { sum: 3, mult: 2, div: 0, sub: -1 };

  Behavior:
  ```javascript
  arrayGenerator('keys', { sum: 3, mult: 2, div: 1, sub: 0 ​​}) // [ 'sum', 'mult', 'div', 'sub' ]
  arrayGenerator('values', { sum: 3, mult: 2, div: 1, sub: 0 ​​}) // [ 3, 2, 1, 0 ]
  arrayGenerator('entries', { sum: 3, mult: 2, div: 1, sub: 0 ​​}) // [ [ 'sum', 3 ], [ 'mult', 2 ], [ 'div', 1 ] , [ 'sub', 0 ] ]
  ```
  The `objPlayground.spec.js` file contains the tests for `calculator` and `arrayGenerator` already implemented. Implement the functions in the `src/objPlayground.js` file so that it meets the proposed tests.

  **What will be evaluated**

  - It will be evaluated if the `calculator` function returns the expected values;
  - It will be evaluated if the `arrayGenerator` function returns the expected values.

</details>



### 8. Implement the `myCounter` function

<details>
  <summary>The myCounter function has two nested loops that insert values ​​into an array. As we can see, they add values ​​to the array until its stop condition.</summary></br>

   Fix the `myCounter` function, without eliminating any of the repeat loops, so that the function returns the correct array. The `myCounter.spec.js` file contains the tests for `myCounter` already implemented. Implement the function in the `src/myCounter.js` file so that it meets the proposed tests.

  **What will be evaluated**

  - It will be validated if the `myCounter` function returns the expected data according to what is implemented in the test.

</details>


### 9. Implement the test cases for the `getCharacter` function

<details>

  <summary>The `getCharacter` function takes a string representing the name of a character and returns an object containing its name, class and phrases.</summary></br>

  ```javascript
  getCharacter('Arya');
  ```

  **Returns:**

  ```javascript
  {
    name: 'Arya Stark',
    class: 'Rogue',
    phrases: ['Not today', 'A girl has no name.']
  }
  ```

  This function is already implemented in the `src/getCharacter.js` file. Write at least six tests for this function in the `tests/getCharacter.spec.js` file to ensure that the implementation of `getCharacter` is correct.

  **What will be evaluated**

  - It will be validated if, in the test of the `getCharacter` function, when receiving a string, the function return is as expected - according to the table presented in the test file.
  - It will be validated if in the test of the `getCharacter` function, when not receiving any parameter, the function return is `undefined`.
  - It will be validated if the test of the `getCharacter` function checks if the parameter is case sensitive.
