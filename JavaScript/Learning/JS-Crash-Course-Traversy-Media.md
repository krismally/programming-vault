# JS Crash Course - Traversy Media
## [Video](https://www.youtube.com/watch?v=hdI2bqOjy3c&list=PLillGF-RfqbYeckUaD1z6nviTp31GLTH8&index=3)

#### Template Literals
- gives ability to interpolate string with JS
- Syntax - `My age is ${age}`
- Surround string with backticks instead of quotations

#### Props & Methods
- Properties don't have paranthesis while methods do
	- ex. `arr.length` is a property `arr.slice()` is a method
- Methods are functions that are associated with objects

#### Arrays
- Unlike other languages, in JS arrays don't have an assigned length 
- Can also have different data types and nested arrays inside array

#### Object Literals
- Uses key:value pairs
- Can also contain dif data types and nested object literals
- Use dot ( . ) syntax to access single value
	- ex. `person.firstName;` will access the key "firstName" in the object literal "person"

#### JSON
- Popular data formatting - stands for "JavaScript Object Notation"
- Similar syntactically to object literals
	- dif is that both keys and values are surrounded by double quotes "key": "value"

#### Loops 
##### For Loops
- Take 3 params - 
	1. Assign iterator - `let i = 0;`
	2. Condition to be met for loop to terminate - `i > arr.length;`
	3. Incrementor - `i++`

##### While Loops
- Take 1 param and assign var outside of loop 
	- Param - condition to be met for loop to terminate - `i > 5`
	- Incrementor is inside loop - `i++`

#### High Order Array Methods
- forEach() - for each elem of array, do this 
- map() - returns new array, good for manipulating array vals without changing original array
- filter() - returns vals of array that match specifications
- each method takes a function as the param
- methods can be chained for greater functionality

#### OOP - Object Oriented Programming
- Can use constructor function