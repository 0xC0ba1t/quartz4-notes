
# ➕ Binary Arithmetic

Binary arithmetic is fundamental to computer science. Since computers only understand two states (0 and 1), all calculations must be performed using binary numbers. Understanding how binary addition, subtraction, multiplication, and division work is essential for grasping how processors perform mathematical operations.

---

## 🧮 Binary Addition

Binary addition follows simple rules based on the addition of bits with possible carries:

| Bits Added       | Result Bit | Carry Out |
|------------------|------------|-----------|
| 0 + 0            | 0          | 0         |
| 0 + 1 or 1 + 0   | 1          | 0         |
| 1 + 1            | 0          | 1         |
| 1 + 1 + 1 (carry)| 1          | 1         |

### Explanation

- **0 + 0** equals 0, no carry.
- **1 + 0** or **0 + 1** equals 1, no carry.
- **1 + 1** equals binary `10`, so the sum bit is 0 and carry 1 to the next higher bit.
- When adding three bits (including carry), **1 + 1 + 1** equals binary `11` — sum bit 1, carry 1.

---

### Example: Adding Two 4-Bit Numbers

Add binary `1011` (decimal 11) and `1101` (decimal 13):

Carry:  1 1 1 1
       1 0 1 1
     + 1 1 0 1
     ----------
     1 1 0 0 0

Step-by-step:

| Bit Position | Bits Added         | Result Bit | Carry Out |
|--------------|--------------------|------------|-----------|
| 0 (LSB)      | 1 + 1              | 0          | 1         |
| 1            | 1 + 0 + 1 (carry)  | 0          | 1         |
| 2            | 0 + 1 + 1 (carry)  | 0          | 1         |
| 3 (MSB)      | 1 + 1 + 1 (carry)  | 1          | 1         |

The carry out of 1 is added as the new leftmost bit, giving `11000` (decimal 24).

---

## ⚠️ Overflow in Binary Addition

**Overflow** occurs when the number of bits is insufficient to store the result.

- E.g., adding two 8-bit numbers could generate a 9-bit result.
- The leftmost bit (carry out) may be lost, causing incorrect results.

### Example:

11111111 (255 decimal)

* 00000001 (1 decimal)

---

1 00000000 (256 decimal but only 8 bits stored → 00000000)

The carry is lost, result becomes zero incorrectly.

---

## 🧮 Binary Subtraction

Binary subtraction works similarly to decimal subtraction, with borrowing when subtracting a larger bit from a smaller bit.

| Bits Subtracted | Result Bit | Borrow |
|-----------------|------------|--------|
| 0 - 0           | 0          | 0      |
| 1 - 0           | 1          | 0      |
| 1 - 1           | 0          | 0      |
| 0 - 1           | 1 (borrow) | 1      |

---

### Borrowing Explained:

- If subtracting 0 - 1, you must borrow 1 from the next higher bit.
- Borrowed 1 equals 2 in binary, so 2 - 1 = 1.

---

### Two's Complement Method for Subtraction

Computers typically perform subtraction by adding the two's complement (negative) of a number.

Steps to find two's complement of a binary number:

1. Invert all bits (flip 0 → 1, 1 → 0).
2. Add 1 to the inverted number.

Example: Find two's complement of `0101` (5 decimal):

0101 → invert → 1010
1010 + 1 = 1011 (which represents -5 in two's complement)

To subtract `5 - 3`:

- Convert 3 to two's complement: `0011` → invert `1100` +1 → `1101`
- Add to 5: `0101 + 1101 = 1 0010` (ignore carry out)
- Result: `0010` = 2 decimal

---

## 🧮 Binary Multiplication

Binary multiplication resembles decimal multiplication, but simpler because bits are only 0 or 1.

| Multiplying Bits | Result  |
|------------------|---------|
| 0 × 0            | 0       |
| 0 × 1            | 0       |
| 1 × 0            | 0       |
| 1 × 1            | 1       |

---

### Example: Multiply 101 (5 decimal) by 11 (3 decimal)

   101
  × 11
  -----
   101    (101 × 1)
   1010    (101 × 1 shifted left)
   -----
   1111    (15 decimal)

---

## 🧮 Binary Division

Binary division is similar to long division in decimal:

1. Compare divisor to leftmost bits of dividend.
2. Subtract if divisor ≤ bits.
3. Bring down next bit and repeat.

---

## Summary Table

| Operation     | Description                          | Example                          |
|---------------|------------------------------------|---------------------------------|
| Addition      | Add bits with carries               | `1011 + 1101 = 11000`           |
| Subtraction   | Borrow or use two’s complement      | `1010 - 0011 = 0111`            |
| Multiplication| Multiply bits and shift             | `101 × 11 = 1111`               |
| Division      | Repeated subtraction and shifting  | `1100 ÷ 10 = 110`               |

---

>📝 Notes

- Binary arithmetic is the basis of all computer calculations.
- Two's complement simplifies subtraction and negative number representation.
- Overflow must be handled carefully to avoid errors.

---

>💡 Tips

- Practice adding and subtracting binary numbers until comfortable.
- Use truth tables to understand hardware adders.
- Remember that shifting bits left or right multiplies or divides by 2, useful in multiplication/division.

---

>✅ Good to Know

- CPUs use circuits called **half adders** and **full adders** for binary addition.
- The overflow flag in CPUs indicates when arithmetic results exceed bit capacity.
- Binary multiplication and division are foundational to more complex arithmetic operations inside processors.

---