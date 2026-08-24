## Python String Methods

| Method          | Name            | Definition                                   | Example                                   |
| --------------- | --------------- | -------------------------------------------- | ----------------------------------------- |
| `.upper()`      | Uppercase       | Converts all characters to uppercase         | `"hello".upper()` → `"HELLO"`             |
| `.lower()`      | Lowercase       | Converts all characters to lowercase         | `"HELLO".lower()` → `"hello"`             |
| `.capitalize()` | Capitalize      | Makes the first character uppercase          | `"hello".capitalize()` → `"Hello"`        |
| `.title()`      | Title Case      | Capitalizes the first character of each word | `"hello world".title()` → `"Hello World"` |
| `.swapcase()`   | Swap Case       | Swaps uppercase and lowercase                | `"Hello".swapcase()` → `"hELLO"`          |
| `.strip()`      | Strip           | Removes whitespace from both ends            | `" hello ".strip()` → `"hello"`           |
| `.lstrip()`     | Left Strip      | Removes whitespace from the left             | `" hello".lstrip()` → `"hello"`           |
| `.rstrip()`     | Right Strip     | Removes whitespace from the right            | `"hello ".rstrip()` → `"hello"`           |
| `.replace()`    | Replace         | Replaces part of a string                    | `"hello".replace("h", "j")` → `"jello"`   |
| `.split()`      | Split           | Breaks a string into a list                  | `"a,b,c".split(",")` → `['a', 'b', 'c']`  |
| `.join()`       | Join            | Combines items into a string                 | `"-".join(["a", "b"])` → `"a-b"`          |
| `.find()`       | Find            | Returns the position of a substring          | `"hello".find("e")` → `1`                 |
| `.index()`      | Index           | Returns the position of a substring          | `"hello".index("e")` → `1`                |
| `.count()`      | Count           | Counts occurrences                           | `"hello".count("l")` → `2`                |
| `.startswith()` | Starts With     | Checks if string starts with something       | `"hello".startswith("he")` → `True`       |
| `.endswith()`   | Ends With       | Checks if string ends with something         | `"hello".endswith("lo")` → `True`         |
| `.isdigit()`    | Is Digit        | Checks if all characters are digits          | `"123".isdigit()` → `True`                |
| `.isalpha()`    | Is Alphabetic   | Checks if all characters are letters         | `"Hello".isalpha()` → `True`              |
| `.isalnum()`    | Is Alphanumeric | Checks if characters are letters/numbers     | `"Hello123".isalnum()` → `True`           |
| `.isspace()`    | Is Whitespace   | Checks if all characters are whitespace      | `"   ".isspace()` → `True`                |
| `.islower()`    | Is Lowercase    | Checks if characters are lowercase           | `"hello".islower()` → `True`              |
| `.isupper()`    | Is Uppercase    | Checks if characters are uppercase           | `"HELLO".isupper()` → `True`              |

**Important:** String methods generally **return a new string** rather than modifying the original.

```python
name = "hello"

name.upper()

print(name)  # hello
```

To keep the result:

```python
name = name.upper()

print(name)  # HELLO
```
## Python — Escape Characters

| Character     | Name              | Definition                                | Example                |
| ------------- | ----------------- | ----------------------------------------- | ---------------------- |
| `\'`          | Single Quote      | Inserts a single quote                    | `'It\'s OK'`           |
| `\"`          | Double Quote      | Inserts a double quote                    | `"He said \"Hi\""`     |
| `\\`          | Backslash         | Inserts a backslash                       | `"C:\\Users"`          |
| `\n`          | New Line          | Creates a new line                        | `"Hello\nWorld"`       |
| `\t`          | Tab               | Inserts a tab                             | `"Name:\tJohn"`        |
| `\r`          | Carriage Return   | Moves cursor to the beginning of the line | `"Hello\rWorld"`       |
| `\b`          | Backspace         | Moves one character backward              | `"Hell\bo"`            |
| `\` + newline | Line Continuation | Continues a string/code on the next line  | `"Hello \`<br>`World"` |

---

## Python — String Indexing / Characters

Python strings are **zero-indexed**, meaning the first character is at index `0`.

```python
text = "Python"
```

| Expression | Result | Definition               |
| ---------- | ------ | ------------------------ |
| `text[0]`  | `P`    | First character          |
| `text[1]`  | `y`    | Second character         |
| `text[2]`  | `t`    | Third character          |
| `text[-1]` | `n`    | Last character           |
| `text[-2]` | `o`    | Second-to-last character |

---

## Python — String Slicing

Syntax:

```python
string[start:stop:step]
```

**Important:** `stop` is **not included**.

| Expression   | Result     | Definition                          |
| ------------ | ---------- | ----------------------------------- |
| `text[0:2]`  | `"Py"`     | Index 0 up to, but not including 2  |
| `text[2:5]`  | `"tho"`    | Index 2 up to, but not including 5  |
| `text[:3]`   | `"Pyt"`    | Start from beginning                |
| `text[3:]`   | `"hon"`    | Continue to the end                 |
| `text[:]`    | `"Python"` | Copy the whole string               |
| `text[::2]`  | `"Pto"`    | Every 2nd character                 |
| `text[::3]`  | `"Ph"`     | Every 3rd character                 |
| `text[::-1]` | `"nohtyP"` | Reverse the string                  |
| `text[-3:]`  | `"hon"`    | Last 3 characters                   |
| `text[:-2]`  | `"Pyth"`   | Everything except last 2 characters |
