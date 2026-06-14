# ⚖️ Variables & Data Types Comparison

This document details how Python, Rust, and TypeScript manage variable declarations, naming bindings, primitive types, type safety, and mutability.

---

## 🐍 Python Variables
In Python, variables are labels bound to values in memory. Types are evaluated at runtime, making Python **dynamically typed**.

* **Declaration**: Simply assign with `=`. No keywords needed.
* **Mutability**: Ints, floats, strings, booleans, and tuples are immutable. Lists, dictionaries, and sets are mutable.
* **Type System**: Strongly, dynamically typed. You cannot perform operations on incompatible types (e.g., adding a string to an integer will trigger a `TypeError`).

---

## 🦀 Rust Variables
Rust bindings are strict. Types are resolved at compile time, making Rust **statically and strongly typed**.

* **Declaration**: Declared using the `let` keyword.
* **Mutability**: **Immutable by default**. To change a variable's value, you must declare it with the `let mut` keyword.
* **Type System**: Statically typed with robust type inference. If the compiler cannot determine the type, you must supply an explicit type annotation (e.g., `let x: i32 = 10;`).

---

## 📘 TypeScript Variables
TypeScript overlays static analysis on top of JavaScript. Variables follow JavaScript runtime scoping rules but are checked at compilation.

* **Declaration**: Declared using `const` (for constants) or `let` (for re-assignable values).
* **Mutability**: `const` prevents re-assigning the variable name, but objects and arrays declared with `const` remain internally mutable unless frozen (`Object.freeze`) or marked `readonly`.
* **Type System**: Statically typed with structural checking. Types are erased at runtime during compile-to-JavaScript process.

---

## 💻 Comparative Code Snippets

### Variable Assignment

```python
# Python: Dynamic and re-assignable
name = "Alice"
age = 25
age = 26  # Re-assignment is valid
```

```rust
// Rust: Immutable by default, statically checked
let name: &str = "Alice";
let mut age: i32 = 25;
age = 26; // Valid because of `mut`
```

```typescript
// TypeScript: Statically typed, const vs let
const name: string = "Alice";
let age: number = 25;
age = 26; // Valid because of `let`
```

---

## 🔑 Key Differences at a Glance

| Feature | Python | Rust | TypeScript |
| :--- | :--- | :--- | :--- |
| **Typing Style** | Dynamic | Static | Static |
| **Default Binding** | Re-assignable | Immutable | Re-assignable (if `let`), Const (if `const`) |
| **Type Coercion** | Weak coercion (Strict) | No coercion (Strict) | Weak coercion in JS runtime |
| **Memory Allocation** | Managed (Garbage Collected) | Managed (Compile-time Ownership) | Managed (Garbage Collected) |
| **Null-Safety** | `None` (Runtime checked) | `Option<T>` (Compile-time checked) | StrictNullChecks compiler config |

---

## 🎯 Practice Tasks

1. **Task 1: Basic Calculations**
   - Declare variables representing a user name, basic wage (decimal), and days worked (integer) in all three languages.
   - Calculate total payment.
   - Print output text containing types and calculation results.

2. **Task 2: Testing Mutability**
   - Attempt to re-assign an immutable variable in Rust and TypeScript, and observe the compilation errors.
   - Attempt to append an item to an immutable tuple in Python and see the runtime exception.
