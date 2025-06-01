
Binary is the language of computers — all digital circuits, memory, and processors work with binary digits (bits).

## What is Binary?

- Base-2 number system.
- Uses only two digits: `0` and `1`.
- Each bit represents an increasing power of 2, from right to left.

---

## Column Headings (8-bit example):

|128|64|32|16|8|4|2|1|
|-|-|-|-|-|-|-|-|

Each column represents 2ⁿ, where n is the position index starting from 0 on the right.

---

## How Binary Represents Data

- **Logic gates** inside CPUs work with `on/off` states, represented as 1s and 0s.
- Binary is used to encode:
  - Machine instructions
  - Memory addresses
  - Numerical values
  - Characters (via encoding schemes like ASCII, Unicode)

---

### Example: Converting Binary `10110110` to Denary

1. Identify place values:

|1|0|1|1|0|1|1|0|
|-|-|-|-|-|-|-|-|
|128|64|32|16|8|4|2|1|

2. Sum the place values where bits = 1:

128 + 0 + 32 + 16 + 0 + 4 + 2 + 0 = **182**

---

### Binary Arithmetic

Binary arithmetic follows simple rules that mimic decimal arithmetic but are simplified to two digits.

---

### Common Uses

- Logic circuits
- Low-level data storage
- Machine code instructions

---

>📝 **Note**: Transistors are the physical implementation of bits — their switching states (on/off) correspond to 1 and 0.

>💡 **Tip**: Practice converting between binary and denary frequently for fluency.

>⚠️ **Warning**: Binary numbers can become very long for large values, which is why hexadecimal is often used for readability.

>✅ **Good to Know**: 1 byte = 8 bits, often grouped together for data.

---

### Binary Data Example

| Binary        | Denary | Hexadecimal |
|---------------|--------|-------------|
| 00000001      | 1      | 01          |
| 11111111      | 255    | FF          |
| 10000000      | 128    | 80          |

---

