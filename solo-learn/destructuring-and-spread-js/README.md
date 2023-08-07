### Destructuring and Spread operators
#### Difficulty : easy
1. Write a function called `getFirstAndLast` that takes an array of numbers as input and returns an array containing the first and last elements of the input array using destructuring.

example :
```js
const inputArray = [1, 2, 3, 4, 5];
const result = getFirstAndLast(inputArray);
console.log(result); // Output: [1, 5]
```

2. Consider the following object:
```js
const person = {
  first_name: 'John',
  last_name: 'Doe',
  age: 30
}
```
Using destructuring, create three variables `firstName`, `lastName`, and `age` and assign them the values from the person object. Then, print these variables.

#### Difficulty medium

1. Write a function called `mergeArrays` that takes multiple arrays as arguments and uses the spread operator to merge them into a single array.

example :
```js
const arr1 = [1, 2, 3];
const arr2 = [4, 5, 6];
const arr3 = [7, 8, 9];
const result = mergeArrays(arr1, arr2, arr3);
console.log(result); // Output: [1, 2, 3, 4, 5, 6, 7, 8, 9]
```

#### Difficulty Hard

1. Write a function called swapVariables that takes two variables a and b as input and uses destructuring to swap their values.

Example:
```js
let a = 10;
let b = 20;
swapVariables(a, b);
console.log(a, b); // Output: 20, 10
```


#### Difficulty extra hard

1. Write a function called `flattenObject` that takes a nested object as input and returns a flattened object with keys representing the full path to the leaf values in the input object.
You can assume that the input object is a nested object with no circular references.

example :
```js
const nestedObject = {
  a: 1,
  b: {
    c: 2,
    d: {
      e: 3,
      f: 4,
    },
  },
  g: 5,
};
const result = flattenObject(nestedObject);
console.log(result);
// Output: { 'a': 1, 'b.c': 2, 'b.d.e': 3, 'b.d.f': 4, 'g': 5 }
```

#### Part two

2. Imagine you have a complex data structure that represents a company's employees.
The structure is as follows:

```js
const companyData = {
  companyName: 'TechCo',
  ceo: {
    firstName: 'John',
    lastName: 'Doe',
    age: 45,
    address: {
      city: 'New York',
      country: 'USA',
    },
  },
  employees: [
    {
      firstName: 'Alice',
      lastName: 'Johnson',
      age: 30,
      address: {
        city: 'San Francisco',
        country: 'USA',
      },
    },
    {
      firstName: 'Bob',
      lastName: 'Smith',
      age: 35,
      address: {
        city: 'London',
        country: 'UK',
      },
    },
    // Add more employee objects as needed
  ],
};
``` 
Your task is to use destructuring and spread operators to extract specific information from the `companyData` object and create new variables for the following:

1. Extract the `ceo` object and assign it to a variable named `ceoData`.
2. Extract the `employees` array and assign it to a variable named `employeeData`.
3. Extract the `firstName`, `lastName`, and `age` of the CEO and assign them to variables named `ceoFirstName`, `ceoLastName`, and `ceoAge`, respectively.
4. Extract the `firstName`, `lastName`, and `age` of the first employee in the employees array and assign them to variables named `firstEmployeeFirstName`, `firstEmployeeLastName`, and `firstEmployeeAge`, respectively.
5. Extract the `city` and `country` of the CEO's address and assign them to variables named `ceoCity` and `ceoCountry`, respectively.
6. Extract the `city` and `country` of the first employee's address and assign them to variables named `firstEmployeeCity` and `firstEmployeeCountry`, respectively.

Now, print all the variables you created to see if you successfully extracted the data from the `companyData` object.
