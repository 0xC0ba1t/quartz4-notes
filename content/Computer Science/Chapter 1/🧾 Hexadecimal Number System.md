
Hexadecimal is a base-16 number system, widely used in computing because it compactly represents binary data.

---

## Basics of Hexadecimal

- Uses 16 digits: `0-9` and `A-F`.
- Letters represent values from 10 (`A`) to 15 (`F`).

---

### Column Headings (5-digit example):

| 65536 | 4096 | 256 | 16  | 1   |
| ----- | ---- | --- | --- | --- |

Each column represents powers of 16.

---

## Why Use Hexadecimal?

- More compact than binary.
- Easier for humans to read.
- Common in memory addresses, color codes, and network IDs.

---

### Example: Hex `2F3A` to Denary

| 2               | F               | 3           | A           |
| --------------- | --------------- | ----------- | ----------- |
| 2 × 4096 = 8192 | 15 × 256 = 3840 | 3 × 16 = 48 | 10 × 1 = 10 |

Sum: 8192 + 3840 + 48 + 10 = **12090**

---

## Common Uses

### Error Codes

Memory dumps and debugging use hex to identify addresses easily.

>💡 *Think of error codes like postcodes telling where the crash occurred.*

---

### HTML Colour Codes

- RGB colors are represented as 6 hex digits: `#RRGGBB`
- Each pair represents Red, Green, Blue intensities (`00` to `FF`)

Example: `#FF0000` = full red, no green or blue.

---

### MAC Addresses

- Unique device identifiers for network interfaces.
- Format: `NN-NN-NN-DD-DD-DD`
- First 3 bytes = manufacturer ID, last 3 = device serial number.

>📝 **Note**: 48-bit MAC addresses allow ~281 trillion unique devices.

>⚠️ **Warning**: MAC addresses can be spoofed by attackers for malicious purposes.

---

### IP Addresses

- IPv4: 32 bits (4 groups of 8-bit numbers, 0-255)
- IPv6: 128 bits (8 groups of 16 bits, hex separated by colons)

---

### Types of IP Addresses

- **Static**: Permanent; used by servers and some devices.
- **Dynamic**: Assigned temporarily via DHCP; common for home users.

---

>📝 **Note**: IPv4 addresses are nearly exhausted; IPv6 adoption is ongoing worldwide.

>✅ **Good to Know**: IPv6 supports security features like encryption and authentication by default.

---

