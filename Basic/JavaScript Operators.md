# JavaScript Operators

JavaScript operators are special symbols or keywords used to perform operations on operands (values or variables) to produce a result.

Operators are fundamental in implementing business logic, performing comparisons, handling conditions, and manipulating data in applications.


⭐ Types of Operators in JavaScript

⭐ 1. Arithmetic Operators

Used for mathematical calculations.

```
let a = 10;
let b = 5;

a + b   // 15
a - b   // 5
a * b   // 50
a / b   // 2
a % b   // 0
a ** b  // power

```

⭐ 2. Assignment Operators

Used to assign values.

```
let x = 10;

x += 5;  // x = x + 5
x -= 2;
x *= 3;
x /= 2;

```

⭐ 3. Comparison Operators

Return boolean.

```
10 > 5     // true
10 < 5     // false
10 >= 10   // true
10 == "10" // true (loose equality)
10 === "10" // false (strict equality)

```

⭐ Equality Concept

Loose Equality (==)

Performs type coercion

```
0 == false  // true
"" == false // true
```
Strict Equality (===)

Checks value + type

```
```

⭐ 4. Logical Operators

```
true && false   // false
true || false   // true
!true           // false

```

⭐ Short-Circuit Behavior

AND Operator

```
const user = isLoggedIn && fetchUser();
```


OR Operator

```
const name = inputName || "Guest";

```

⭐ 5. Nullish Coalescing Operator

Handles only `null` and `undefined`.

```
const name = inputName ?? "Guest";

```
Better than `||`

```
0 || 10   // 10 ❌
0 ?? 10   // 0 ✅

```

⭐ 6. Ternary Operator

Inline condition writing.

```
let result = age > 18 ? "Adult" : "Minor";
```

⭐ 7. Spread Operator

Copies values.

```
const arr2 = [...arr1];

```

⭐ 8. Rest Operator

Collects values.

```
function sum(...nums) {
  return nums.reduce((a,b) => a + b);
}

```

⭐ 9. Optional Chaining

Prevents crash.

```
user?.address?.city

```