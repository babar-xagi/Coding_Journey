# 🐍 Python Foundations

This module covers the entry-level concepts of Python: environment setup, dynamic variables, primitive data types, and standard outputs.

---

## 📝 Concept Summary

Python is an interpreted, high-level, dynamically typed programming language.
1. **Dynamic Typing**: Variable types are bound to the runtime object, not the variable name itself.
2. **Mutability**: Primitive values (integers, floats, strings, booleans) are immutable, while containers like lists and dictionaries are mutable.
3. **No Compiler Step**: Code is interpreted directly by the Python runtime (e.g., CPython).

---

## 💻 Code Snippets

```python
# 1. Variable declaration
user_age = 25              # int
pi_value = 3.14159         # float
username = "Alice"         # str
is_active = True           # bool

# 2. Type reflection
print(type(user_age))  # <class 'int'>

# 3. Re-assignment (Dynamic typing)
user_age = "twenty-five"
print(type(user_age))  # <class 'str'>

# 4. Basic Console Output
print(f"User {username} is active: {is_active}")
```

---

## 🎯 Mini Practice Exercise

Create a script `foundations.py` that declares variables representing a product (name, price, quantity, active status). Calculate the total value, format it to 2 decimal places, and print a receipt block to the terminal.

```python
# exercises/foundations.py
product_name = "System Console"
price = 49.99
quantity = 3
is_available = True

if is_available:
    total_cost = price * quantity
    print(f"Receipt for: {product_name}")
    print(f"Quantity: {quantity} @ ${price} each")
    print(f"Total Cost: ${total_cost:.2f}")
else:
    print(f"Product {product_name} is currently out of stock.")
```
