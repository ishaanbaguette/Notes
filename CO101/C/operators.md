**Date:** 21 Aug  

**Subject:** CO101  

---

## Topics Covered
- [Arithmetic Operators](#arithmetic-operators)  
- [Logical Operators](#logical-operators)  
- [Relational Operators](#relational-operators)  
- [Assignment Operators](#assignment-operators)  
- [Bitwise Operators](#bitwise-operators)  
- [Bit Shifts](#bit-shifts)  
- [Conditional (Ternary) Operator](#conditional-ternary-operator)  
- [Comma Operator](#comma-operator)  
- [Precedence](#precedence)  
- [TLDR](#tldr)  
- [Useful Stuff](#useful-stuff)  


---

### Types of Operators
- Arithmetic  
- Logical  
- Relational  
- Assignment  
- Bitwise  
- Conditional (Ternary)
- Comma operator

---

## Arithmetic Operators
| **Operator** | **Symbol** | **Example** |
|--------------|------------|-------------|
| Addition     | `+`        | `5 + 3 = 8` |
| Subtraction  | `-`        | `5 - 3 = 2` |
| Multiplication | `*`      | `5 * 3 = 15` |
| Division     | `/`        | `6 / 3 = 2` |
| Modulus      | `%`        | `5 % 2 = 1` |

---

## Logical Operators
| **Operator** | **Symbol** | **Example** |
|--------------|------------|-------------|
| AND          | `&&`       | `(5 > 3 && 2 < 4) → true` |
| OR           | `\|\|`       | `(5 > 3 \|\| l 2 > 4) → true` |
| NOT          | `!`        | `!(5 > 3) → false` |

---

## Relational Operators
| **Operator** | **Symbol** | **Example** |
|--------------|------------|-------------|
| Equal to     | `==`       | `5 == 5 → true` |
| Not equal to | `!=`       | `5 != 3 → true` |
| Greater than | `>`        | `5 > 3 → true` |
| Less than    | `<`        | `5 < 3 → false` |
| Greater or equal | `>=`   | `5 >= 5 → true` |
| Less or equal    | `<=`   | `3 <= 5 → true` |

---

## Assignment Operators
| **Operator** | **Symbol** | **Example** |
|--------------|------------|-------------|
| Assign       | `=`        | `x = 5` |
| Add & assign | `+=`       | `x += 3  // x = x + 3` |
| Subtract & assign | `-=`  | `x -= 2  // x = x - 2` |
| Multiply & assign | `*=`  | `x *= 4  // x = x * 4` |
| Divide & assign   | `/=`  | `x /= 2  // x = x / 2` |
| Modulus & assign  | `%=`  | `x %= 2  // x = x % 2` |

---

## Bitwise Operators
| **Operator** | **Symbol** | **Example (5=0101, 3=0011)** |
|--------------|------------|-------------------------------|
| AND          | `&`        | `5 & 3 = 1 (0001)` |
| OR           | `\|`       | `5 \| 3 = 7 (0111)` |
| XOR          | `^`        | `5 ^ 3 = 6 (0110)` |
| NOT          | `~`        | `~5 = -6` |
| Left Shift   | `<<`       | `5 << 1 = 10` |
| Right Shift  | `>>`       | `5 >> 1 = 2` |

---

## Bit Shifts
Only works on **integers** (not floats).  

- **Left Shift (`x << n`)**  
 Shifts all bits of `x` to the left by `n` positions, filling the right side with `0`.  
 Equivalent to multiplying by `2^n`.  

  Example:
```
5 << 1 = 10
(0101 << 1 → 1010)
```

- **Right Shift (`x >> n`)**  
Shifts all bits of `x` to the right by `n` positions.  
Equivalent to integer division by `2^n` (floor division).  

Example:
```
9 >> 2 = 2
(1001 >> 2 → 0010)
```

---

## Conditional (Ternary) Operator
| **Operator** | **Syntax** | **Example** |
|--------------|------------|-------------|
| Ternary      | `? :`      | `(5 > 3) ? 10 : 20 → 10` |

---

## Comma Operator

- Evaluates expressions **from left to right**.  
- **Final value = result of the rightmost expression.**  
- **Precedence** is lower than assignment (`=`).  

### Example
```c
int x, y;

x = (2, 3, 4);   // x = 4
y = 2, 3, 4;     // y = 2

printf("%d %d", x, y);  // Output: 4 2
```
---

## Precedence

- Arithmetic > Relational > Logical

- ! (logical NOT) > && (logical AND) > || (logical OR)

- Comma has the lowest precedence
---


# TLDR
- **Arithmetic** → basic math  
- **Logical** → `&&`, `||`, `!` for true/false conditions  
- **Relational** → comparisons like `==`, `<`, `>=`  
- **Assignment** → `=`, `+=`, `-=` etc.  
- **Bitwise** → works on binary bits (`&`, `\|`, `^`, `~`, `<<`, `>>`)  
- **Conditional** → shortcut for `if-else` using `? :`  
- **Comma operator**
`(a, b, c)` → evaluates all, result = `c`
```
x = (1, 2, 3); // x = 3
x = 1, 2, 3;   // x = 1
```

---

# Useful Stuff
- **XOR (`^`)** → “different bits = 1, same = 0” → good for toggling.  
Example: `a ^ a = 0`  
- **NOT (`~x`)** → flips all bits → result is `-(x+1)` in signed ints.  
Example: `~5 = -6`  
- **Bitwise AND (`&`)** → check even/odd:  
`x & 1 → 0 (even), 1 (odd)`  
- **Logical vs Bitwise:**  
- Logical → works on conditions/booleans (`true/false`)  
- Bitwise → works on actual bits (`0/1`)  

---
