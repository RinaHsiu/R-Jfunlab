# 31 What Are Built-in Functions?

**Built-in functions** are special tools that come with Python (or other programming languages) and are ready to use without any extra setup. Think of them like the default tools in a toolbox—already there, easy to grab, and super handy for solving problems.

---

## Imagine This:
- Imagine a magical toolbox that has tools for everything you need. For example:
  - Need to add numbers? There’s a tool for that!
  - Want to know how many toys are in a box? There’s a tool for counting too!

In Python, these tools are called **built-in functions**. They are already built into the language, so you don’t need to build them yourself.

---

## Examples of Built-in Functions

Here are some built-in functions in Python and what they do:

1. **`print()`**:
   - **What It Does**: Shows text or information on the screen.
   - **Example**:
     ```python
     print("Hello, World!")
     ```
     **Output**:
     ```
     Hello, World!
     ```

2. **`len()`**:
   - **What It Does**: Counts how many items are in a list or how many letters are in a word.
   - **Example**:
     ```python
     toys = ["car", "doll", "ball"]
     print(len(toys))  # Counts the toys
     ```
     **Output**:
     ```
     3
     ```

3. **`max()`** and **`min()`**:
   - **What They Do**: Find the biggest and smallest numbers in a list.
   - **Example**:
     ```python
     numbers = [3, 7, 1, 9]
     print(max(numbers))  # Biggest number
     print(min(numbers))  # Smallest number
     ```
     **Output**:
     ```
     9
     1
     ```

4. **`type()`**:
   - **What It Does**: Tells you what kind of data something is.
   - **Example**:
     ```python
     print(type(10))       # Number
     print(type("apple"))  # Text
     ```
     **Output**:
     ```
     <class 'int'>
     <class 'str'>
     ```

---

## Why Are Built-in Functions Useful?
- **Save Time**: You don’t need to write your own tools for common tasks—they're already there!
- **Easy to Use**: Built-in functions are simple and beginner-friendly.
- **Powerful**: They let you do cool things with just one line of code.

---

## How Do You Use Built-in Functions?
1. **Write the function name** (like `print` or `len`).
2. **Put parentheses** `()` after the function name.
3. **Give it the information it needs inside the parentheses**.

---

## Summary
- **Built-in functions** are like tools that come with Python for free.
- You use them to do common tasks like showing text (`print`), counting items (`len`), or finding the biggest number (`max`).
- They make programming easier and more fun!

So, the next time you use a built-in function, imagine you're grabbing a cool tool from your magical Python toolbox!

# 32 Arguments
# What Are Arguments?

In programming, **arguments** are pieces of information that you give to a function so it can perform its task. Think of arguments like the ingredients you give to a recipe. The recipe (function) needs these ingredients (arguments) to make the final dish (result).

---

## Example: Baking a Cake
Imagine you have a recipe for baking a cake. The recipe might need:
- Flour
- Sugar
- Eggs

These ingredients are like arguments. Without them, the recipe wouldn’t work.

Similarly, in programming, a function might need arguments to complete its job.

---

## How Do Arguments Work in Python?
When you call a function, you pass the arguments inside the parentheses `()`. The function uses these arguments to perform a task.

### Example 1: A Simple Function with Arguments
```python
def greet(name):
    print("Hello, " + name)

greet("Alice")  # Output: Hello, Alice
greet("Bob")    # Output: Hello, Bob
