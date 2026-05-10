# Spectral Channel Integrity (SCI): Deterministic Color Channel Separation

**A model for maintaining the independence of RGB data channels on physical media.**

## The Problem: Spectral Crosstalk
In digital systems, RGB channels are perfectly isolated. Each pixel emits light independently, allowing for seamless data stream separation. However, when transitioning to physical media (print, painting), this independence collapses.

Physical objects reflect light rather than emit it. Pigments do not operate in clean spectral bands—they possess broad reflection and absorption "tails." A red pigment will inevitably reflect some green light, and blue will bleed into red. This is known as **spectral crosstalk**, which corrupts the data structure.

## The Solution
The SCI model eliminates inter-channel interference, allowing color channels to maintain their functional independence in a subtractive environment.

### Core Principle: Equilibrium by the Weakest Link
Pigments differ in the strength of their spectral response. The "weakest" component in the system is typically a complex **Violet**. This pigment becomes the **Spectral Limiter** for the entire system.

The entire palette is calibrated to stay within the physical limits of this Violet anchor. The system becomes tonally constrained, but gains a crucial property: **Operational Separability**. Channels can be decoded at the physics level—via narrow-band light or optical filters—without relying on software "guesswork" or ML post-processing.

## The Experiment
To eliminate bias toward specific printers or ink types, the model was tested using **acrylic paint on canvas**:
1. **Reference Swatch:** Created a deterministic swatch where R, G, and B patches showed clear isolation under narrow-band RGB light.
2. **Calibration:** Established reference levels based on the spectral response of the anchor pigment.
3. **Physical Matrix:** A multi-channel color QR code was manually painted as a test medium.
4. **Scanner Interface:** Developed a real-time analysis tool to observe how the camera sensor perceives channel interaction.

### Key Finding
The experiment demonstrated that while camera sensors introduce their own software-level color distortions, the fundamental problem is solvable at the **model level**. The focus is not on a "special decoding algorithm," but on a **color model** that ensures channel separation *before* the camera even captures the image.

## Applications (Beyond QR)
While multi-channel color codes (tripling data density) are the most obvious use case, the principle is universal:
* **Ornamental Encoding (QRnament, Batch 00-30):** Embedding data into aesthetically complex patterns.
* **Spectral Art:** Physical objects that change behavior/content under different spectral lighting (the origin of this research).
* **Spectral Steganography:** Hidden data channels, invisible to the eye but readable by instruments.

## Limitations
This is an experimental technique. It requires calibration for specific pigments (specifically the spectral response of the violet anchor). However, the method itself is universal: any medium that can be described by a spectral curve can be normalized using this principle.

## Resources
* **Theory (Zenodo):** [Preprint: Spectral Channel Integrity](https://zenodo.org/records/19633526)
* **Generator #1:** [QR.G.B.-ART (Artistic QR)](https://astra31415926.github.io/QR.G.B.-ART/)
* **Generator #2:** [QRnament2 (Ornamental)](https://astra31415926.github.io/QRnament2/)
* **Project Portfolio:** [Spectral Design & Art](https://astra31415926.github.io/#contacts)

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
