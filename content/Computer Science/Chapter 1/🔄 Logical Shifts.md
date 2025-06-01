
Shifts move bits left or right in a binary number.

---

## Left Shift

- Moves all bits to the left by n positions.
- Vacated bits on the right are filled with zeros.
- Equivalent to multiplying by 2ⁿ.

---

## Right Shift

- Moves all bits to the right by n positions.
- Vacated bits on the left are filled with zeros.
- Equivalent to integer division by 2ⁿ (ignores remainder).

---

### Example: Left shift 00010110 by 2

Before: 00010110 (22 decimal)

After: 01011000 (88 decimal)

---

>💡 **Tip**: Used in low-level programming for fast multiplication/division.

---

>⚠️ **Note**: Logical shifts differ from arithmetic shifts, which preserve the sign bit for signed integers.

---

