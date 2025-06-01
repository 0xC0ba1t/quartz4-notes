
Computers must convert analogue sounds and images into digital data to process, store, and transmit them.

---

## Sound

Sound is a continuous analogue signal caused by air vibrations. To digitize sound, computers use **Analogue to Digital Converters (ADCs)**.

### Sampling

- Sampling is measuring the amplitude of sound waves at regular intervals.
- The **sampling rate** is how many times per second the sound is measured, in Hertz (Hz).

>💡 CD quality audio uses **44,100 samples per second (44.1 kHz)**.

---

### Sampling Resolution (Bit Depth)

- Represents how precisely each sample is measured.
- Higher bit depth = more possible amplitude values.
- CD quality uses **16-bit resolution**, meaning each sample can have 2¹⁶ = 65,536 levels.

---

### Effects of Sampling Rate and Bit Depth

| Quality Factor    | Effect                               |
|-------------------|------------------------------------|
| Higher Sampling Rate | More accurate sound reproduction, larger file size |
| Higher Bit Depth     | More dynamic range, less noise and distortion |

---

### Digital Sound Example

- A music clip sampled at 44.1 kHz with 16-bit depth.
- The digital file contains thousands of samples, each represented as a binary number.

---

## Images

Digital images consist of **pixels** arranged in a grid.

### Pixels

- Each pixel stores **colour** and **brightness**.
- Colour stored using **colour depth** — number of bits per pixel.

---

### Colour Depth

- The number of bits per pixel defines how many different colours can be displayed.
- Common depths:

| Bits per Pixel | Number of Colours             |
|----------------|------------------------------|
| 1-bit          | 2 (black and white)           |
| 8-bit          | 256 colours                   |
| 16-bit         | 65,536 colours (High Color)  |
| 24-bit         | ~16.7 million colours (True Color) |

>📝 Example: 8-bit colour depth means the pixel can be one of 256 colours, usually from a palette.

---

### Image Resolution

- Number of pixels in width × height (e.g., 1920 × 1080).
- Higher resolution = sharper images but larger file sizes.

---

### File Formats

- **JPEG** — uses lossy compression, ideal for photos.
- **PNG** — uses lossless compression, supports transparency.
- **GIF** — supports animation, limited to 256 colours.

---

>📝 Notes

- Sound and image quality depend heavily on sampling and colour depth.
- Compression is often used to reduce file sizes but may lose quality.

---

>💡 Tips

- Choose appropriate sampling rates and bit depths depending on use.
- Use lossless compression when quality is critical.
- Understand trade-offs between quality and file size.

---

>✅ Good to Know

- WAV files store uncompressed sound data.
- MP3 and AAC use lossy compression.
- BMP files store uncompressed images, resulting in large file sizes.

---
