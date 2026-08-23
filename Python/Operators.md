## Python Basics — Operators

| Keywords / Symbol | Name                    | Definition                                       | Example                       |
| ----------------- | ----------------------- | ------------------------------------------------ | ----------------------------- |
| `=`               | Assignment              | Assigns a value                                  | `x = 10`                      |
| `+`               | Addition                | Adds values                                      | `10 + 5` → `15`               |
| `-`               | Subtraction             | Subtracts values                                 | `10 - 5` → `5`                |
| `*`               | Multiplication          | Multiplies values                                | `10 * 5` → `50`               |
| `/`               | Division                | Divides values                                   | `10 / 5` → `2.0`              |
| `//`              | Floor division          | Divides and removes the decimal part             | `10 // 3` → `3`               |
| `%`               | Modulus                 | Returns the remainder                            | `10 % 3` → `1`                |
| `**`              | Exponentiation          | Raises a number to a power                       | `2 ** 3` → `8`                |
| `==`              | Equal                   | Checks if values are equal                       | `5 == 5` → `True`             |
| `!=`              | Not equal               | Checks if values are different                   | `5 != 3` → `True`             |
| `>`               | Greater than            | Checks if left is greater                        | `5 > 3` → `True`              |
| `<`               | Less than               | Checks if left is smaller                        | `5 < 3` → `False`             |
| `>=`              | Greater than or equal   | Checks if left is greater/equal                  | `5 >= 5` → `True`             |
| `<=`              | Less than or equal      | Checks if left is smaller/equal                  | `3 <= 5` → `True`             |
| `and`             | Logical AND             | Both conditions must be true                     | `x > 0 and x < 10`            |
| `or`              | Logical OR              | At least one condition must be true              | `x < 0 or x > 10`             |
| `not`             | Logical NOT             | Reverses a Boolean value                         | `not True` → `False`          |
| `in`              | Membership              | Checks if a value exists in a collection         | `"a" in "apple"` → `True`     |
| `not in`          | Not membership          | Checks if a value doesn't exist                  | `"z" not in "apple"` → `True` |
| `is`              | Identity                | Checks if two variables refer to the same object | `x is y`                      |
| `is not`          | Not identity            | Checks if they refer to different objects        | `x is not y`                  |
| `+=`              | Add and assign          | Adds then assigns                                | `x += 5`                      |
| `-=`              | Subtract and assign     | Subtracts then assigns                           | `x -= 5`                      |
| `*=`              | Multiply and assign     | Multiplies then assigns                          | `x *= 5`                      |
| `/=`              | Divide and assign       | Divides then assigns                             | `x /= 5`                      |
| `//=`             | Floor divide and assign | Floor-divides then assigns                       | `x //= 5`                     |
| `%=`              | Modulus and assign      | Gets remainder then assigns                      | `x %= 5`                      |
| `**=`             | Exponent and assign     | Raises then assigns                              | `x **= 2`                     |

### The most important ones to memorize first

```text
=   +   -   *   /   //   %   **
==  !=  >   <   >=  <=
and  or  not
in   not in
```

The others can be learned naturally as you encounter them.

# Python Operators

## 1. Arithmetic Operators

| Keyword / Symbol | Name           | Definition                       | Example         |
| ---------------- | -------------- | -------------------------------- | --------------- |
| `+`              | Addition       | Adds two values                  | `5 + 3` → `8`   |
| `-`              | Subtraction    | Subtracts one value from another | `5 - 3` → `2`   |
| `*`              | Multiplication | Multiplies values                | `5 * 3` → `15`  |
| `/`              | Division       | Divides values                   | `5 / 2` → `2.5` |
| `//`             | Floor Division | Divides and rounds down          | `5 // 2` → `2`  |
| `%`              | Modulus        | Returns the remainder            | `5 % 2` → `1`   |
| `**`             | Exponentiation | Raises a value to a power        | `5 ** 2` → `25` |

---

## 2. Comparison Operators

| Keyword / Symbol | Name                  | Definition                         | Example           |
| ---------------- | --------------------- | ---------------------------------- | ----------------- |
| `==`             | Equal                 | Checks if values are equal         | `5 == 5` → `True` |
| `!=`             | Not Equal             | Checks if values are different     | `5 != 3` → `True` |
| `>`              | Greater Than          | Checks if left is greater          | `5 > 3` → `True`  |
| `<`              | Less Than             | Checks if left is smaller          | `5 < 3` → `False` |
| `>=`             | Greater Than or Equal | Checks if left is greater or equal | `5 >= 5` → `True` |
| `<=`             | Less Than or Equal    | Checks if left is smaller or equal | `3 <= 5` → `True` |

---

## 3. Boolean / Logical Operators

| Keyword | Name | Definition                          | Example              |
| ------- | ---- | ----------------------------------- | -------------------- |
| `and`   | AND  | Both conditions must be true        | `x > 0 and x < 10`   |
| `or`    | OR   | At least one condition must be true | `x < 0 or x > 10`    |
| `not`   | NOT  | Reverses the Boolean result         | `not True` → `False` |

---

## 4. Bitwise Operators

| Symbol | Name        | Definition               | Example                |                |
| ------ | ----------- | ------------------------ | ---------------------- | -------------- |
| `&`    | AND         | Compares bits using AND  | `5 & 3` → `1`          |                |
| `      | `           | OR                       | Compares bits using OR | `5 \| 3` → `7` |
| `^`    | XOR         | Compares bits using XOR  | `5 ^ 3` → `6`          |                |
| `~`    | NOT         | Inverts the bits         | `~5` → `-6`            |                |
| `<<`   | Left Shift  | Shifts bits to the left  | `5 << 1` → `10`        |                |
| `>>`   | Right Shift | Shifts bits to the right | `5 >> 1` → `2`         |                |

**You don't need to prioritize these yet.** They're more important when you get into lower-level programming, networking, or cybersecurity.

---

## 5. Identity Operators (`is`)

| Keyword  | Name         | Definition                                            | Example      |
| -------- | ------------ | ----------------------------------------------------- | ------------ |
| `is`     | Identity     | Checks whether two variables refer to the same object | `x is y`     |
| `is not` | Not Identity | Checks whether they refer to different objects        | `x is not y` |

> `is` checks **identity**, while `==` checks **value equality**.

Example:

```python
a = [1, 2, 3]
b = a
c = [1, 2, 3]

print(a is b)  # True
print(a is c)  # False
```

Why?

```text
a → [1, 2, 3] ← b
c → [1, 2, 3]
```

`b = a` means **both variables point to the exact same object**, so:

```python
a is b  # True
```

`c` has the same contents, but it's a **different object**, so:

```python
a is c  # False
```

But:

```python
a == c  # True
```

because their **values are the same**.

---

## 6. Membership Operators (`in`)

| Keyword  | Name           | Definition                                    | Example                       |
| -------- | -------------- | --------------------------------------------- | ----------------------------- |
| `in`     | Membership     | Checks whether a value exists in a collection | `"a" in "apple"` → `True`     |
| `not in` | Not Membership | Checks whether a value doesn't exist          | `"z" not in "apple"` → `True` |

---

## 7. Ternary Operator

Python doesn't have a separate `? :` operator. Instead, it uses a **conditional expression**:

| Syntax                  | Name                   | Definition                                  | Example                                          |
| ----------------------- | ---------------------- | ------------------------------------------- | ------------------------------------------------ |
| `x if condition else y` | Conditional Expression | Returns one value if true, another if false | `age = 20` → `"Adult" if age >= 18 else "Minor"` |

Example:

```python
age = 20
status = "Adult" if age >= 18 else "Minor"

print(status)
# Adult
```
