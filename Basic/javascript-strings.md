# JavaScript Strings

A string is a sequence of characters.

It is used to store text.

```
"Hello"
"Sangam"
"JavaScript"
"123" → this is still a string because it is inside quotes

```

```
let name = "Sangam";
let city = 'Pune';

console.log(name);
console.log(city);

```


How to Create a String

1. Double quotes

```
let str1 = "Hello";

```

2. single Quote

```
let str2 = 'Hello';

```

3. Backticks

```
let str3 = `Hello`;

```

String vs Number

```
let a = "100";
let b = 100;

console.log(a); 
console.log(b);


"100" is a string
100 is a number

```

Check type

```
let a = "100";
let b = 100;

console.log(typeof a); // string
console.log(typeof b); // number

```

Empty String

```
let str = "";
console.log(str);
console.log(typeof str);

```

String with Spaces

```
let text = "Hello World";
console.log(text);

```

String Length

To find how many characters are in a string, use .length

```
let str = "Hello";
console.log(str.length);

```

o/p:

```
5

```

Access Characters from a String

Each character in a string has a position called index.

Index starts from 0.

```
let str = "Hello";

Indexes:

H → 0
e → 1
l → 2
l → 3
o → 4

```

Access by index

```
let str = "Hello";

console.log(str[0]); // H
console.log(str[1]); // e
console.log(str[2]); // l
console.log(str[3]); // l
console.log(str[4]); // o

```

```
let str = "Hello";
console.log(str[str.length - 1]);

```

Strings are Immutable

mmutable means:you cannot directly change original string characters.

```
let str = "Hello";
str[0] = "Y";

console.log(str);

```

```
Hello

```

Combine Strings

This is called concatenation.

```
let firstName = "Sangam";
let lastName = "Shinde";

let fullName = firstName + " " + lastName;

console.log(fullName);

```

```
Sangam Shinde

```

```
let a = "Hello";
let b = "World";

console.log(a + b);
console.log(a + " " + b);


```

```
HelloWorld
Hello World

```

Add String and Number

```
let str = "Age: ";
let age = 23;

console.log(str + age);

```
JavaScript converts number to string here.
```
Age: 23

```

Template Literals

Template literals use backticks.

```
let name = "Sangam";
let age = 23;

let text = `My name is ${name} and I am ${age} years old`;

console.log(text);

```

```
My name is Sangam and I am 23 years old

```




Common String Methods

1. `toUpperCase()`

Converts all letters to uppercase.

```
let str = "hello";
console.log(str.toUpperCase());

```

```
HELLO

```

2. `toLowerCase()`

Converts all letters to lowercase.

```
let str = "HELLO";
console.log(str.toLowerCase());

```

```
hello

```


3. `trim()`
Removes spaces from start and end.

```
let str = "   hello   ";
console.log(str.trim());

```

```
hello

```

4. `includes()`

Checks if a string contains something.

```
let str = "I love JavaScript";

console.log(str.includes("JavaScript")); // true
console.log(str.includes("Python")); // false

```

5. `startsWith()`

Checks if string starts with given text.

```
let str = "JavaScript";

console.log(str.startsWith("Java")); // true
console.log(str.startsWith("Script")); // false

```

6. `endsWith()`

Checks if string ends with given text.

```
let str = "JavaScript";

console.log(str.endsWith("Script")); // true
console.log(str.endsWith("Java")); // false

```

7. `indexOf()`

Returns index of first matching character or word.


```
let str = "Hello World";
console.log(str.indexOf("o"));

```

```
4

```

If not found:

```
console.log(str.indexOf("z"));

```

```
-1

```

8. `slice()`

Used to get part of a string.

```
let str = "JavaScript";

console.log(str.slice(0, 4));

```

```
Java

```

9. `replace()`

Replace part of string.

```
let str = "I love Java";
let newStr = str.replace("Java", "JavaScript");

console.log(newStr);

```

Output:

```
I love JavaScript

```

10. `repeat()`

Repeats string multiple times.

```
let str = "Hi ";
console.log(str.repeat(3));

```

```
Hi Hi Hi

```


Method Chaining

You can use multiple methods together.

```
let str = "   hello world   ";

let result = str.trim().toUpperCase();

console.log(result);

```


```
HELLO WORLD

```
Escape Characters in Strings

Sometimes we want quotes inside a string.

```
let str = "He said, \"Hello\"";
console.log(str);

```

```
He said, "Hello"

```

Common escape characters

\"
double quote inside double-quoted string

\'
single quote inside single-quoted string

\n
new line

```
let str = "Hello\nWorld";
console.log(str);

```

```
Hello
World

```

Convert Other Types to String

`String()`

```
let num = 123;
let result = String(num);

console.log(result); // "123"
console.log(typeof result); // string

```
`split()`
 converts string into array.

 ```
 let str = "apple,banana,mango";
 let arr = str.split(",");

 console.log(arr);

 ```
 

 ```
 ["apple", "banana", "mango"]

 ```

 