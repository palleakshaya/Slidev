---
# You can also start simply with 'default'
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://cover.sli.dev
# some information about your slides (markdown enabled)
title: Welcome to Slidev
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# apply unocss classes to the current slide
class: text-center
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# https://sli.dev/guide/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations#slide-transitions
transition: slide-left
# enable MDC Syntax: https://sli.dev/guide/syntax#mdc-syntax
mdc: true
---

# OPERATORS

---

<v-clicks>

Operators are symbols or keywords that perform operations on variables and values.
They are categorized into 3 types

</v-clicks>

<v-clicks>

1.  Unary Operators

</v-clicks>

<v-clicks>

2.  Binary Operators

</v-clicks>

<v-clicks>

3.  Ternary Operator

</v-clicks>

<v-clicks>

#### 1. Unary operators: Requires only one operand

</v-clicks>
  
  <v-clicks>

i. Unary Plus (➕): Converts its operand into a number.

  </v-clicks>

  <v-clicks>

```js
let numberString = "123";
let num = +numberString; // Unary plus operator
console.log(num); // Output: 123 (converted to a number)
```

  </v-clicks>

  <v-clicks>

ii. Unary Minus (➖): Negates its operand.

  </v-clicks>

  <v-clicks>

```js
let x = 10;
let y = -x; // Unary minus operator
console.log(y); // Output: -10
```

  </v-clicks>

---

  <v-clicks>

iii. Increment (➕➕): Increases the numeric value of its operand by 1.
Can be used as a prefix (++i) or postfix (i++). <br>

     a. Pre-Increment:

```js
let a = 5;
let b = ++a; // Pre-increment operator
console.log(a); // Output: 6
console.log(b); // Output: 6
```

  </v-clicks>

 <v-clicks>

     b. Post-Increment:

```js
let c = 8;
let d = c++; // Post-increment operator
console.log(c); // Output: 9
console.log(d); // Output: 8
```

</v-clicks>

  <v-clicks>

iv. Decrement (➖➖❕): Decreases the numeric value of its operand by 1.
Can be used as a prefix (--i) or postfix (i--).

  </v-clicks>

  <v-clicks>

```js
let x = 10;
console.log(x); // Output: 10
x--; // Decrement operator, decreases the value of x by 1
console.log(x); // Output: 9
```

  </v-clicks>

---

  <v-clicks>

v. Logical NOT (❕): Returns false if its single operand can be converted to true; otherwise, returns true.

  </v-clicks>

  <v-clicks>

```js
let flag = true;
let opposite = !flag; // Logical NOT operator
console.log(opposite); // Output: false
```

</v-clicks>

  <v-clicks>

vi. Bitwise NOT (~): Inverts all the bits of its operand.

  </v-clicks>

<v-clicks>

```js
let num = 7; // Binary: 0111
let bitwiseNotResult = ~num;
console.log(bitwiseNotResult); // Output: -8
```

</v-clicks>

  <v-clicks>

vii. Typeof: Returns a string indicating the type of the unevaluated operand.

  </v-clicks>

  <v-clicks>

```js
let num = 10;
console.log(typeof num); // Output: "number"
```

  </v-clicks>

  <v-clicks>
  
   viii. Void: Discards the return value of an expression.

  </v-clicks>

  <v-clicks>

```js
void console.log("Hello, World!");
```

  </v-clicks>

---

<v-clicks>

2. Binary Operators: Requires two operands

</v-clicks>

<v-clicks>

- Arithmetic Operators: <br>

</v-clicks>

<v-clicks>

i. Addition(+) <br>

</v-clicks>

<v-clicks>

```js
let a = 5;
let b = 3;
let addition = a + b;
console.log(addition); // Output: 8
```

  </v-clicks>

<v-clicks>

ii.Subtraction(-) <br>

</v-clicks>

<v-clicks>

```js
let a = 5;
let b = 3;
let sub = a - b;
console.log(sub); // Output: 2
```

  </v-clicks>

<v-clicks>

iii.Multiplication(\*) <br>

</v-clicks>

<v-clicks>

```js
let a = 5;
let b = 3;
let mul = a * b;
console.log(mul); // Output: 15
```

  </v-clicks>

---

<v-clicks>

iv.Division(/) <br>

</v-clicks>

<v-clicks>

```js
let a = 5;
let b = 3;
let div = a / b;
console.log(div); // Output: 1.6666666666666667
```

  </v-clicks>

<v-clicks>

v.Modulus(%)

</v-clicks>

<v-clicks>

```js
let a = 5;
let b = 3;
let mod = a % b;
console.log(mod); // Output: 2
```

  </v-clicks>

<v-clicks>

- Comparison Operators:

</v-clicks>

<v-clicks>

i. Equal to (==) <br>
ii.Not equal to (!=) <br>
iii.Strict equal to (===) & Strict not equal to (!==) <br>
v.Greater than (>) <br>
vi.Less than (<) <br>
vii.Greater than or equal to (>=) <br>
viii.Less than or equal to (<=)

</v-clicks>

---

<v-clicks>

Example:

</v-clicks>

<v-clicks>

```js
let x = 5;
let y = 3;
console.log(x > y); // Output: true
console.log(x < y); // Output: false
console.log(x >= y); // Output: true
console.log(x <= y); // Output: false
let a = "apple";
let b = "banana";
console.log(a === b); // Output: false
console.log(a !== b); // Output: true
let num = 10;
console.log(num == "10"); // Output: true (loose equality, coerces types)
console.log(num === "10"); // Output: false (strict equality, checks types)
```

</v-clicks>

<v-clicks>

- Logical Operators:

</v-clicks>

<v-clicks>

i. Logical AND (&&): Returns true if both operands are true.

</v-clicks>

<v-clicks>

```js
let x = 5;
let y = 3;
console.log(x > 0 && y > 0); // Output: true
console.log(x > 0 && y < 0); // Output: false
```

</v-clicks>

---

<v-clicks>

ii.Logical OR (||): Returns true if at least one of the operands is true.

</v-clicks>

<v-clicks>

```js
let a = 10;
let b = 0;
console.log(a > 0 || b < 0); // Output: true
console.log(a < 0 || b < 0); // Output: false
```

</v-clicks>

<v-clicks>

- Bitwise Operators

</v-clicks>

<v-clicks>

i.Bitwise AND (&) <br>
ii.Bitwise OR (|) <br>
iii.Bitwise XOR (^) <br>
iv.Left shift (<<) <br>
v.Signed right shift (>>) <br>
vi.Zero-fill right shift (>>>)

</v-clicks>

---

<v-clicks>

Example:

```js
// Bitwise AND (&)
let x = 5; // Binary: 0101
let y = 3; // Binary: 0011
console.log(x & y); // Output: 1 (Binary:0001)

// Bitwise OR (|)
let a = 5; // Binary: 0101
let b = 3; // Binary: 0011

console.log(a | b); // Output: 7 (Binary: 0111)

// Bitwise XOR (^)
let m = 5; // Binary: 0101
let n = 3; // Binary: 0011

console.log(m ^ n); // Output: 6 (Binary: 0110)

// Bitwise Left Shift (<<)
let num = 5; // Binary: 0101

console.log(num << 1); // Output: 10 (Binary: 1010)

// Bitwise Right Shift (>>)
let num2 = 10; // Binary: 000000000000000000000000
```

</v-clicks>

---

<v-clicks>

- Assignment Operators:

</v-clicks>

<v-clicks>

i.Assignment (=) <br>
ii.Addition assignment (+=) <br>
iii.Subtraction assignment (-=) <br>
iv.Multiplication assignment (\*=) <br>
v.Division assignment (/=) <br>
vi.Modulus assignment (%=) <br>

</v-clicks>

<v-clicks>

Example:

```js
let x = 5;
console.log(x); // Output: 5
x += 3; // Addition Assignment (x = x + 3)
console.log(x); // Output: 8
x -= 2; // Subtraction Assignment (x = x - 2)
console.log(x); // Output: 6
x *= 4; // Multiplication Assignment (x = x * 4)
console.log(x); // Output: 24
x /= 3; // Division Assignment (x = x / 3)
console.log(x); // Output: 8
x %= 5; // Modulus Assignment (x = x % 5)
console.log(x); // Output: 3
```

</v-clicks>

---

<v-clicks>

3. Ternary Operator: It is a conditional operator

</v-clicks>

<v-clicks>

The syntax can be written as,

</v-clicks>

<v-clicks>

```js
condition ? expression1 : expression2;
```

</v-clicks>

<v-clicks>

Example:

```js
let age = 25;
let message = age >= 18 ? "Adult" : "Minor";

console.log(message); // Output: "Adult"
```

</v-clicks>
