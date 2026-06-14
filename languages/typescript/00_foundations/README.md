# 📘 TypeScript Foundations

This module covers the entry-level concepts of TypeScript: the TypeScript compiler (tsc), type annotations, variable bindings (`let`/`const`), and basic runtime interactions.

---

## 📝 Concept Summary

TypeScript is a typed superset of JavaScript that compiles (transpiles) to plain JavaScript.
1. **Static Typing**: Type annotations are checked by the compiler, but are completely erased from the compiled output JavaScript (type erasure).
2. **Variable Binding**: Follows JavaScript rules. `const` creates block-scoped immutable bindings, while `let` creates block-scoped mutable variables.
3. **Target Options**: The compilation configuration (`tsconfig.json`) dictates whether target JavaScript matches ES5, ES6, ES2020, etc.

---

## 💻 Code Snippets

```typescript
// 1. Immutable declaration
const username: string = "Alice";
const isActive: boolean = true;

// 2. Mutable declaration
let userAge: number = 25;
userAge = 26; // Valid

// 3. Types list
const tags: string[] = ["admin", "student"];

// 4. Output Formatting
console.log(`User ${username} is active: ${isActive} (Age: ${userAge})`);
```

---

## 🎯 Mini Practice Exercise

Create a simple typescript script `foundations.ts` that defines variables representing an item name, price, quantity, and available status. Compiles it using `tsc` and logs a formatted printout block.

```typescript
// src/foundations.ts
const itemName: string = "System Console";
const price: number = 49.99;
const quantity: number = 3;
const isAvailable: boolean = true;

if (isAvailable) {
  const totalCost: number = price * quantity;
  console.log(`Receipt for: ${itemName}`);
  console.log(`Quantity: ${quantity} @ $${price.toFixed(2)} each`);
  console.log(`Total Cost: $${totalCost.toFixed(2)}`);
} else {
  console.log(`Product ${itemName} is currently out of stock.`);
}
```
