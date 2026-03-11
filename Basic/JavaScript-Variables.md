# JavaScript Variables

- A variable in JavaScript is a named container used to store data values in memory so that they can be accessed, modified, and reused throughout the execution of a program.

- Variable means a box where we store value.

JavaScript provides three ways:
- var
- let
- const

## let Variable
- ``` let ``` is block-scoped variable declaration keyword introduced in ES6 that allows reassignment but prevents redeclaration within the same scope.

```
let age = 25;

age = 26; // allowed 

```


```
if (true) {
  let name = "Sangam";
}

console.log(name); // ❌ ReferenceError

```

⭐ const Variable

- ``` const  ``` is a block-scoped variable declaration keyword that prevents reassignment after initialization.

```
const pi = 3.14;

pi = 4; // ❌ Error

```

Const does NOT make object immutable.

```

const user = { name: "A" };

user.name = "B"; // ✅ allowed

```
Only reference is fixed.

⭐ var Variable (Legacy)

var is function-scoped variable declaration keyword that allows redeclaration and hoisting, which can lead to unexpected behavior in large applications.

```
var x = 10;

var x = 20; // allowed

```

⭐ Hoisting Behavior

Variables declared with var are hoisted and initialized with undefined.

```
console.log(a); // undefined
var a = 10;

```

But `let` and `const` are hoisted in Temporal Dead Zone.

```
console.log(b); // ❌ error
let b = 10;

```

⭐ Naming Rules

- Must start with letter, `_` or `$`
- Cannot start with number
- Cannot use reserved keywords