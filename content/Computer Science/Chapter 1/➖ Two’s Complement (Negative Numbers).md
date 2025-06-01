
Two’s complement is the standard way computers represent signed integers.

---

## Why Two’s Complement?

- Enables addition and subtraction of negative numbers using the same binary arithmetic.
- Avoids having a separate sign bit.
- Simplifies hardware design.

---

## How to Find Two’s Complement

1. Write the number’s binary representation.
2. Flip every bit (0 → 1, 1 → 0).
3. Add 1 to the result.

---

### Example: Represent -5 in 8-bit two’s complement

1. +5 in binary: `00000101`
2. Flip bits: `11111010`
3. Add 1: `11111011` (this is -5)

---

## Convert back to positive:

1. Flip bits of negative number.
2. Add 1.
3. Convert to decimal.

---

>⚠️ **Common Mistake**: Forgetting to flip all bits before adding 1.

---

>✅ **Good to Know**: Two’s complement allows easy detection of overflow and simplifies arithmetic circuits.

---

