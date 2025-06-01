
Data compression reduces the size of files or data streams to save storage space and speed up transmission.

---

## Why Compress Data?

- Saves storage space on devices.
- Speeds up data transfer over networks.
- Reduces bandwidth consumption, which is cost-effective.

---

## Types of Compression

### Lossy Compression

- Permanently removes some data deemed less important.
- Used where perfect accuracy is not necessary (multimedia).
- Common formats:
  - Audio: MP3, AAC
  - Video: MPEG-4, H.264
  - Images: JPEG

>⚠️ **Note:** Once data is lost, it cannot be recovered, potentially reducing quality.

---

### Lossless Compression

- Compresses data without losing any original information.
- Used for text, software files, and images needing exact restoration.
- Common algorithms:
  - Run-Length Encoding (RLE)
  - Huffman Coding
  - Lempel-Ziv-Welch (LZW)

---

### Run-Length Encoding (RLE)

- Works by replacing repeated sequences with a count and value.
- Example: `AAAABBBCC` becomes `4A3B2C`.
- Efficient for data with many repeating characters.

---

### Huffman Coding

- Uses variable-length codes for characters.
- More frequent characters get shorter codes.
- Builds a binary tree based on frequency for encoding.

---

### Lempel-Ziv-Welch (LZW)

- Replaces repeated sequences with references to dictionary entries.
- Used in GIF and ZIP compression.

---

## Advantages and Disadvantages

| Type        | Advantages                           | Disadvantages                   |
|-------------|------------------------------------|--------------------------------|
| Lossy       | High compression ratios, smaller files | Loss of quality, irreversible |
| Lossless    | No loss of data, exact recovery    | Lower compression ratios, larger files |

---

## Real-World Examples

| Format | Compression Type | Use Case                    |
|--------|------------------|-----------------------------|
| ZIP    | Lossless         | Software, documents          |
| PNG    | Lossless         | Web images with transparency|
| MP3    | Lossy            | Music streaming             |
| JPEG   | Lossy            | Digital photos              |

---

>📝 Notes

- Choice of compression depends on application requirements.
- Lossy is suitable for multimedia where small loss is acceptable.
- Lossless is critical for executables, text files, and sensitive data.

---

>💡 Tips

- Always back up original files before compressing with lossy algorithms.
- Check if the software supports the compression format you want.
- Consider the trade-off between file size and quality.

---

>✅ Good to Know

- Some video codecs combine lossy and lossless techniques.
- Compression speeds depend on algorithm complexity and hardware.
- Decompression must exactly reverse compression in lossless methods.

---
