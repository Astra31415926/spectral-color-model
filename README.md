Technology that Preserves the Structure of Color Channels in Print
Problem
On a screen, it's simple: red, green, and blue channels do not interfere with each other. Each pixel glows independently.

On paper or canvas, it's different. Pigments cannot be "purely red" or "purely blue." Each has broad "tails" of reflection and absorption. Red pigment always reflects a little bit of green, and blue reflects red.

This is called spectral crosstalk. Data from one channel "pollutes" the other.

Solution
The model eliminates inter-channel interference (crosstalk), allowing color channels to maintain independence in a subtractive environment.

How it Works
Core principle: Equilibrium by the weakest link.

Pigments are not equal in spectral response strength. The "weakest" is a complex Violet. It becomes the spectral limiter of the entire system.

The entire palette is calibrated so as not to exceed the limits of this Violet. The system becomes tonally limited, but acquires a key property:

Channels become operationally separable. They can be decoded at the level of physics—through light or filters—without software "guesswork."

Experiment
To exclude bias toward a specific printer or type of ink, I worked with acrylic paint on canvas.

Created a reference swatch with a deterministic response—three color spots (R, G, B) clearly separated under narrow-band RGB light.

Calibrated the system—selected reference levels and the spectral limiter.

Painted a color QR code on canvas with the correct colors (as a test medium).

Developed a scanner that shows what the camera sensor sees and allows real-time control over channel interference.

What the Experiment Showed
The reference swatch became an indicator for adjusting the scanner. I saw that the camera itself (at the software level) distorts colors. I was unable to overcome this distortion at the software level.

But the main conclusion: the problem is solved at the model level. The scanner is just a tool for observation; it can be improved. The focus is not on a "special decoding algorithm," but on a color model that makes channels separable before the camera even looks at them.

Where to Apply (Not Only QR)
The most obvious example is multi-channel color codes, where information is stored on three independent channels. But there are more possibilities:

Ornamental Codes (QRnament, Batch 00-30): Embedding data into aesthetically complex patterns.

Light-Sensitive Painting: Physical objects that change behavior under different spectral light. This is where it all began.

Spectral Steganography: Hidden channels, invisible to the eye but readable instrumentally.

Limitations
This is an experimental technique. It requires calibration for specific pigments (specifically the spectral response of violet).

However, the method itself is universal: it is not tied to a specific printer, ink, or scanner. Any medium that can be described by a spectral curve can be normalized using this principle.

Resources
Theory (Zenodo): Preprint: Spectral Channel Integrity

Generator #1 (Art-QR): QR.G.B.-ART

Generator #2 (Ornaments): QRnament2

Project Portfolio: https://astra31415926.github.io/#contacts

---

# Visual Assets & Implementation

### 1. RGB Data Matrices
<p align="left">
  <img src="RGB%20Matrix%20001.png" width="120" />
  <img src="RGB%20Matrix%20002.png" width="120" />
  <img src="RGB%20Matrix%20003.png" width="120" />
  <img src="RGB%20Matrix%20004.png" width="120" />
  <img src="RGB%20Matrix%20005.png" width="120" />
  <img src="RGB%20Matrix%20006.png" width="120" />
  <img src="RGB%20Matrix%20007.png" width="120" />
  <img src="RGB%20Matrix%20008.png" width="120" />
</p>

### 2. Ornamental QR Evolution (Batch 00-30)
<p align="left">
  <img src="ornamental_qr_00.png" width="100" />
  <img src="ornamental_qr_01.png" width="100" />
  <img src="ornamental_qr_02.png" width="100" />
  <img src="ornamental_qr_03.png" width="100" />
  <img src="ornamental_qr_04.png" width="100" />
  <img src="ornamental_qr_05.png" width="100" />
  <img src="ornamental_qr_06.png" width="100" />
  <img src="ornamental_qr_07.png" width="100" />
  <img src="ornamental_qr_08.png" width="100" />
  <img src="ornamental_qr_09.png" width="100" />
  <img src="ornamental_qr_10.png" width="100" />
  <img src="ornamental_qr_11.png" width="100" />
  <img src="ornamental_qr_12.png" width="100" />
  <img src="ornamental_qr_13.png" width="100" />
  <img src="ornamental_qr_14.png" width="100" />
  <img src="ornamental_qr_15.png" width="100" />
  <img src="ornamental_qr_16.png" width="100" />
  <img src="ornamental_qr_17.png" width="100" />
  <img src="ornamental_qr_18.png" width="100" />
  <img src="ornamental_qr_19.png" width="100" />
  <img src="ornamental_qr_20.png" width="100" />
  <img src="ornamental_qr_21.png" width="100" />
  <img src="ornamental_qr_22.png" width="100" />
  <img src="ornamental_qr_23.png" width="100" />
  <img src="ornamental_qr_24.png" width="100" />
  <img src="ornamental_qr_25.png" width="100" />
  <img src="ornamental_qr_26.png" width="100" />
  <img src="ornamental_qr_27.png" width="100" />
  <img src="ornamental_qr_28.png" width="100" />
  <img src="ornamental_qr_29.png" width="100" />
  <img src="ornamental_qr_30.png" width="100" />
</p>

### 3. Physical Artwork Implementation
<p align="left">
  <img src="physical_artwork_01.jpeg" width="200" />
  <img src="physical_artwork_03.png" width="200" />
  <img src="physical_artwork_04.jpeg" width="200" />
  <img src="physical_artwork_05.jpeg" width="200" />
  <img src="physical_artwork_06.jpeg" width="200" />
  <img src="physical_artwork_07.jpeg" width="200" />
  <img src="physical_artwork_08.png" width="200" />
  <img src="physical_artwork_09.jpeg" width="200" />
</p>

### 4. Scanner Interface Analysis
<p align="left">
  <img src="scanner_interface_01.jpg" width="120" />
  <img src="scanner_interface_02.png" width="120" />
  <img src="scanner_interface_03.png" width="120" />
  <img src="scanner_interface_04.png" width="120" />
  <img src="scanner_interface_05.png" width="120" />
  <img src="scanner_interface_06.png" width="120" />
  <img src="scanner_interface_07.png" width="120" />
  <img src="scanner_interface_08.png" width="120" />
  <img src="scanner_interface_09.png" width="120" />
  <img src="scanner_interface_10.png" width="120" />
  <img src="scanner_interface_11.png" width="120" />
  <img src="scanner_interface_12.png" width="120" />
  <img src="scanner_interface_13.png" width="120" />
  <img src="scanner_interface_14.png" width="120" />
  <img src="scanner_interface_15.png" width="120" />
  <img src="scanner_interface_016.png" width="120" />
  <img src="scanner_interface_017.png" width="120" />
</p>

---
**Author:** Mihail Kashkarov
