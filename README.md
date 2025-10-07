# SAR Image Denoising using Multifractal Analysis

A novel approach to **denoise Synthetic Aperture Radar (SAR)** images using **Microcanonical Multiscale Formalism (MMF)** and **Multifractal System** concepts.  
Developed as a **B.Tech Final Year Project** at IIT Patna, this method achieves superior denoising performance, particularly in high noise conditions, compared to existing techniques like SARBM3D.

---

## 📌 Overview

- **Project Title:** SAR Image Denoising  
- **Author:** Rajkishor Ranjan Kumar  
- **Guide:** Dr. Suman Kumar Maji  
- **Institute:** IIT Patna — Department of Computer Science & Engineering

---

## 🌍 Motivation

SAR images are high-resolution satellite images used for applications such as terrain mapping, forest/water body detection, and surveillance. However, they are often degraded by **speckle noise** due to coherent imaging. Traditional filtering methods tend to smooth out important features.

---

## 🧠 Methodology

The project introduces a **multifractal-based denoising** pipeline:

1. **SAR Image Modeling**  
   \( v(x,y) = H(x,y) * u(x,y) + n \)

2. **Multifractal System & MMF**  
   - Compute **Singularity Exponents (SE)** to capture local structure.
   - Extract the **Most Singular Manifold (MSM)** for noise-free features.

3. **Image Reconstruction**  
   - Use **Universal Reconstruction Kernel** in Fourier domain to recover the image from MSM gradient information.

---

## 🧪 Experiments

- **Dataset:** SIPI Image Database  
- **Noise:** Mixed Poisson–Gaussian noise  
- **Metric:** PSNR (Peak Signal-to-Noise Ratio)  
- Compared with **SARBM3D** algorithm.

---

## 🏆 Results

- Consistent **PSNR improvement** across images and noise levels.
- Better edge and texture preservation.
- Demonstrated robustness on **real fluorescence microscopy images**.

---

## 📊 Formula Highlights

**PSNR Calculation:**

\[
\text{PSNR} = 20 \log \frac{\max(s(x))}{\sqrt{\text{MSE}}}
\]

\[
\text{MSE} = \frac{1}{MN} \sum_{i,j} |s(x) - s_r(x)|^2
\]

---

## 🛠️ Future Scope

- Extending the method to **real-time denoising pipelines**.  
- Integration with deep learning frameworks for **hybrid approaches**.  
- Applying MSM to other image restoration tasks.

---

## 📚 References

1. K.S. Shanmungan et al. “A Model for Radar Images and Its Application for Adaptive Digital Filtering of Multiplicative Noise,” *IEEE TPAMI*, 1982.  
2. J.S. Lee. “Digital Image Enhancement and Noise Filtering by Using Local Statistics,” *IEEE TPAMI*, 1980.  
3. C.V. Angelino et al. “A Nonlocal SAR Image Denoising Algorithm Based on LLMMSE Wavelet Shrinkage,” *IEEE TPAMI*, 2010.

---

## 🙏 Acknowledgements

Special thanks to **Dr. Suman Kumar Maji** for his guidance and support throughout the project.

---

## 📬 Contact

**Rajkishor Ranjan Kumar**  
B.Tech — Computer Science & Engineering  
IIT Patna  
📧 rajkishor.cs13@iitp.ac.in
