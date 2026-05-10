# Spectral Channel Integrity (SCI) — Deterministic RGB Normalization

**Physical/Operational separation of independent data channels on reflective media.**

This project introduces a deterministic model for reducing **spectral crosstalk** in multi-channel physical printing. The method was derived from "Spectral Design" (RGB-responsive acrylic painting) to solve the problem of signal leakage between pigments under narrow-band light.

## The Problem: Spectral Crosstalk
In digital environments, R, G, and B channels are discrete. On physical substrates, pigments have broad absorption spectra. Data intended for the Blue channel inevitably "pollutes" the Green channel. Standard approaches (CMYK) rely on software post-processing and ML to "guess" the data, which limits density and reliability.

## The Solution: Physical "Shift Left"
Instead of fixing "dirty" data after scanning, SCI ensures **data integrity during formation (printing)**.

*   **Key Insight:** Using the "weakest" pigment (e.g., Violet acrylic) as a **Spectral Limiter** and tonal anchor.
*   **Normalization:** The entire palette is mathematically normalized against the physical reflection/absorption limits of the anchor pigment under narrow-band RGB light.
*   **Result:** Physical pigments behave like digital pixels. Channels are separated **operationally** (via light or filters) at the hardware level.

## Live Demos & Theory
*   **Theory (Zenodo):** [Spectral Channel Integrity Preprint](https://zenodo.org/records/19633526)
*   **Artistic QR Gen:** [QR.G.B.-ART](https://astra31415926.github.io/QR.G.B.-ART/)
*   **Ornamental QR Gen:** [QRnament2](https://astra31415926.github.io/QRnament2/)

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

### 2. Ornamental QR Evolution
<p align="left">
  <img src="ornamental_qr_00.png" width="100" />
  <img src="ornamental_qr_01.png" width="100" />
  <img src="ornamental_qr_02.png" width="100" />
  <img src="ornamental_qr_03.png" width="100" />
  <img src="ornamental_qr_04.png" width="100" />
  <img src="ornamental_qr_05.png" width="100" />
</p>

### 3. Physical Artwork Implementation
<p align="left">
  <img src="physical_artwork_01.jpeg" width="200" />
  <img src="physical_artwork_03.png" width="200" />
  <img src="physical_artwork_04.jpeg" width="200" />
  <img src="physical_artwork_08.png" width="200" />
</p>

### 4. Scanner Interface Analysis
<p align="left">
  <img src="scanner_interface_01.jpg" width="120" />
  <img src="scanner_interface_02.png" width="120" />
  <img src="scanner_interface_03.png" width="120" />
  <img src="scanner_interface_04.png" width="120" />
</p>

---
**Author:** Mihail Kashkarov — Science Art, Spectral Channel Integrity.
