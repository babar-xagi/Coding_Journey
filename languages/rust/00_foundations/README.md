# 🦀 Rust Foundations

This module covers the entry-level concepts of Rust: compilation, Cargo configurations, type annotations, strict immutability by default, and standard print macros.

---

## 📝 Concept Summary

Rust is a compiled, statically typed, systems programming language.
1. **Immutability by Default**: Variables declared with `let` are immutable. They cannot be changed unless explicitly marked with `mut`.
2. **Static & Safe**: Types are checked at compile-time. Memory safety is checked via ownership and lifetime rules without a garbage collector.
3. **Compilation Step**: Cargo manages compilation, building binary targets into `/target` directories.

---

## 💻 Code Snippets

```rust
fn main() {
    // 1. Immutable declaration
    let username: &str = "Alice";
    let is_active: bool = true;

    // 2. Mutable declaration
    let mut user_age: i32 = 25;
    user_age = 26; // Valid

    // 3. Compile-time constants
    const PI_VALUE: f64 = 3.14159;

    // 4. Output Formatting
    println!("User {} is active: {} (Age: {})", username, is_active, user_age);
}
```

---

## 🎯 Mini Practice Exercise

Write a simple rust program inside a new cargo project. Define variables representing a store item: price (`f64`), count (`u32`), and name (`&str`). Calculate total price, print the result using formatting macros, and check for overflow values.

```rust
// src/main.rs
fn main() {
    let item_name: &str = "System Console";
    let price: f64 = 49.99;
    let quantity: u32 = 3;
    let is_available: bool = true;

    if is_available {
        let total_cost = price * (quantity as f64);
        println!("Receipt for: {}", item_name);
        println!("Quantity: {} @ ${:.2} each", quantity, price);
        println!("Total Cost: ${:.2}", total_cost);
    } else {
        println!("Product {} is currently out of stock.", item_name);
    }
}
```
