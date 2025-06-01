
Converting between number systems is essential to understand and manipulate computer data.

---

## Denary → Binary

Steps:

1. Divide the denary number by 2.
2. Record the remainder (0 or 1).
3. Divide the quotient again by 2.
4. Repeat until quotient is 0.
5. The binary number is the remainders read from bottom to top.

---

### Example: Convert 13 to Binary

| Division | Quotient | Remainder |
|----------|----------|-----------|
| 13 ÷ 2   | 6        | 1         |
| 6 ÷ 2    | 3        | 0         |
| 3 ÷ 2    | 1        | 1         |
| 1 ÷ 2    | 0        | 1         |

Reading bottom up → **1101**

---

>💡 **Tip**: Use a table to keep track; it reduces mistakes.

---

## Hexadecimal → Denary

1. Multiply each hex digit by its place value (powers of 16).
2. Add all results.

---

### Example: `3A` hex to denary

- `3 × 16 = 48`
- `A (10) × 1 = 10`

Sum: 48 + 10 = **58**

---

## Denary → Hexadecimal

1. Divide the denary number by 16.
2. Track remainders.
3. Read remainders bottom-up.

---

### Example: Convert 58 to hex

| Division | Quotient | Remainder |
|----------|----------|-----------|
| 58 ÷ 16  | 3        | 10 (`A`)  |
| 3 ÷ 16   | 0        | 3         |

Reading bottom-up → **3A**

---

>📝 **Note**: This process is analogous to denary → binary conversion but with base 16.

---

