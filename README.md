# Spectral Color Model
**Deterministic normalization for printable color channels and steganographic synthesis**

## The Concept
Standard digital RGB channels are independent, but physical pigments on canvas crosstalk due to spectral overlap. This project implements a deterministic model to isolate and normalize these channels, allowing for stable data embedding (like QR codes) within complex artistic patterns.

## Visual Proof: Ornamental Synthesis
The model transforms utilitarian data into aesthetic ornaments without losing readability.
![Ornamental QR](ornamental_qr_01.jpg)
*Symmetrical ornamental composition generated via spectral synthesis.*

## Physical Implementation
The technology is tested on physical canvases using custom-mixed pigments.
![Physical Canvas](physical_artwork_01.jpg)
*Hand-painted canvas: data integrity is maintained through physical pigment normalization.*

## Spectral Logic & Synthesis
We merge multiple independent data streams into a single color-encoded matrix.
![Synthesis Logic](model_logic_01.png)
*Synthesis process: from three independent QR codes to a single spectral-encoded pattern.*

## Real-time Decoding
A custom scanner isolates R, G, and B channels by applying inverse normalization parameters.
![Scanner Interface](scanner_interface_01.png)
*Scanner UI: adjusting Offset, Gain, and crosstalk coefficients (k1, k2) for perfect extraction.*

## Channel Isolation & Stress Testing
Verification of the model's robustness under different spectral conditions.
![Channel Isolation](channel_separation_01.jpg)
*Isolated R, G, and B responses as seen by the algorithm.*

![Stress Test](red_light_test_01.jpg)
*Robustness test: verifying pigment response under monochromatic lighting.*

## Links & Resources
- **Interactive Demo:** [QR.G.B.-ART](https://astra31415926.github.io/)
- **Full Preprint (Math):** [Zenodo — SCI Universal Model v1.3.0](https://zenodo.org/records/10633526)
- **Author:** [Mihail Kashkarov](https://github.com/Astra31415926) — Spectral Design & Science Art.
