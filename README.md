# Digital Image Processing Pipeline — Bicycle Image Analysis

This project implements a **complete digital image processing system** in Python using **OpenCV, NumPy, and Matplotlib**.  
It was developed as part of the *Image Processing and Analysis (IPA)* coursework to demonstrate understanding of acquisition, enhancement, denoising, segmentation, and feature evaluation techniques.

---

## Overview
The system analyzes a **real-world bicycle image**, simulating various noise types, applying classical filtering and enhancement operations, and evaluating segmentation and extracted features both qualitatively and quantitatively.

---

##  Pipeline Stages
1. **Image Acquisition**  
   - Real image captured and converted to RGB.  
   - Justification: Balanced lighting, diverse edges, and structural clarity of bicycle.

2. **Noise Simulation**  
   - Added *Gaussian* and *Salt-and-Pepper* noise to simulate real-world distortions.  
   - Evaluated noise characteristics and visual impact.

3. **Image Enhancement**  
   - Applied **Histogram Equalization** and **Contrast Stretching**.  
   - Enhanced visibility and contrast for object boundaries.

4. **Denoising and Filtering**  
   - Used **Median** and **Gaussian** filters for noise reduction.  
   - Compared results using **PSNR** and **SSIM** metrics.

5. **Segmentation**  
   - Combined **Otsu Thresholding** and **Canny Edge Detection**.  
   - Isolated the main object and refined with morphological operations.

6. **Feature Evaluation**  
   - Extracted **geometric**, **intensity**, and **color** features:  
     - Area, Perimeter, Aspect Ratio, Compactness, Convexity  
     - Mean and Std of R/G/B and Gray levels  
     - 3D color histogram (512 bins) and 1D RGB histogram (96 bins)

7. **Visualization & Reflection**  
   - Displayed all stages with annotated images.  
   - Quantitatively assessed workflow performance.

---

##  Evaluation Metrics
| Metric | Median Filter | Gaussian Filter |
|:-------|:--------------:|:----------------:|
| **PSNR (dB)** | 16.41 | 15.02 |
| **SSIM** | 0.88 | 0.82 |

---

##  Key Learnings
- Median filtering provides better edge preservation in high-frequency regions.  
- Histogram equalization enhances structural visibility for segmentation.  
- Classical spatial-domain methods remain highly interpretable and effective.

---

##  Tech Stack
- **Python 3**
- **OpenCV**
- **NumPy**
- **Matplotlib**


---

##  Authors
**Tanisha Sriram** and **Srinidhi V G**  
Department of Computer Science Engineering  
Sri Sivasubramaniya Nadar College of Engineering

---

##  References
- Gonzalez & Woods, *Digital Image Processing*, Pearson, 2018  
- Otsu, *IEEE Trans. SMC*, 1979  
- Canny, *IEEE TPAMI*, 1986  
- Haralick et al., *IEEE Trans. SMC*, 1973  

---


### Keywords
`Image Processing` `OpenCV` `Python` `Noise Reduction` `Histogram Equalization` `Segmentation` `Feature Extraction` `PSNR` `SSIM`
