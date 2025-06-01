
Character encoding is how computers represent text as binary numbers. Every letter, digit, punctuation mark, and symbol must be assigned a unique binary code so that computers can store and process text.

---

## ASCII (American Standard Code for Information Interchange)

- Uses **7 bits** to represent **128 unique characters** (values 0–127).
- Covers:
  - English uppercase and lowercase letters (A-Z, a-z).
  - Digits (0-9).
  - Basic punctuation marks and control characters (e.g., newline, tab).

| Character | ASCII Code (Decimal) | Binary        |
|-----------|---------------------|---------------|
| A         | 65                  | 01000001      |
| a         | 97                  | 01100001      |
| 0         | 48                  | 00110000      |

---

### Extended ASCII

- Uses **8 bits** allowing **256 characters**.
- Adds:
  - Accented letters (é, ñ, ü, etc.).
  - Additional symbols (currency signs, box-drawing characters).
- Common in older Western European systems.

>⚠️ **Warning:** Extended ASCII is not standardized globally, causing incompatibility between different systems.

---

## Unicode

- Developed to support **all languages worldwide** in one standard.
- Uses variable-length encoding schemes like **UTF-8**, **UTF-16**, and **UTF-32**.
- Covers over **143,000 characters** including:
  - Latin, Cyrillic, Greek alphabets.
  - Asian scripts (Chinese, Japanese, Korean).
  - Mathematical symbols.
  - Emojis and technical symbols.

### UTF-8 Encoding

- Uses **1 to 4 bytes** per character.
- Backward compatible with ASCII for first 128 characters.
- Most popular encoding on the web.

### UTF-16 Encoding

- Uses **2 or 4 bytes**.
- Common in Windows and Java environments.

---

## Why Use Unicode?

- Ensures text from any language can be represented and exchanged without corruption.
- Essential for global software, websites, and apps.

---

>📝 Notes

- Character encoding errors cause **garbled text**, often called "mojibake".
- When saving files, always know which encoding is used.
- ASCII is a subset of Unicode.

---

>💡 Tips

- Use UTF-8 encoding by default for maximum compatibility.
- When dealing with legacy systems, check if ASCII or extended ASCII is required.
- Understand how bytes translate to characters to debug encoding problems.

---

>✅ Good to Know

- Unicode Consortium maintains the Unicode standard.
- Emojis are part of Unicode.
- Some languages need combining characters for accents, handled by Unicode normalization.

---