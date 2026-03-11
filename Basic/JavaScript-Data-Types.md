# JavaScript Data Types

JavaScript data types define the kind of values that can be stored and manipulated within a program.

They determine how data is represented in memory and how operations can be performed on that data.

JavaScript is a dynamically typed language, meaning variable types are determined at runtime.

Data type means what kind of value we are storing.
- number
- text
- true/false
- object
- array

⭐ Types of Data Types in JavaScript

JavaScript has 2 main categories
- 1.Primitive Data Types
- 2.Non-Primitive (Reference) Data Types

⭐ Primitive Data Types

Primitive values are immutable and stored by value.

⭐ 1. Number

Used for integers and floating point numbers.

```
let age = 25;
let price = 99.99;

```

⭐ 2. String

Represents textual data.

```
let name = "Sangam";
let city = 'Pune';
```

Template string:

```
let msg = `Hello ${name}`;

```

A string in JavaScript is a primitive data type used to represent textual data.
Strings are immutable sequences of characters that can be manipulated using built-in methods and operators.



⭐ 3. Boolean

Represents logical values.

```
let isLoggedIn = true;

```

⭐ 4. Undefined

Variable declared but not assigned.

```
let x;

console.log(x); // undefined

```

⭐ 5. Null

Represents intentional absence of value.

```
let selectedUser = null;

```

⭐ 6. Symbol (Advanced)

Unique identifier mainly used in advanced object properties.

```
const id = Symbol("id");

```

⭐ 7. BigInt

Used for very large integers beyond Number limit.

```
const big = 12345678901234567890n;

```


⭐ Non-Primitive (Reference) Data Types

Stored by reference (memory address).


⭐ Object

Collection of key-value pairs.

```
const user = {
  name: "Sangam",
  age: 26
};

```

⭐ Array

Ordered collection.

```
const skills = ["JS", "React", "Node"];

```

⭐ Function
Functions are also objects in JavaScript.

```
function greet() {
  return "Hello";
}

```

⭐ typeof Operator

Used to check data type.

```
typeof 10          // number
typeof "hi"        // string
typeof true        // boolean
typeof {}          // object
typeof []          // object (important)
typeof null        // object (JS bug)
```