# 🖼️ Hough Transform for Line Detection

This project demonstrates the implementation of the **Hough Transform (HT)** for detecting lines in images. It is a fundamental technique in **digital image processing and computer vision**, widely used for identifying shapes and patterns.

---

## 🚀 Overview

The Hough Transform converts the problem of detecting lines in an image into finding peaks in a parameter space. Instead of detecting collinear points directly, it maps them into **(ρ, θ) space** and identifies intersections.

---

## 📌 Key Concepts

- 📍 **Edge Detection**
  - Uses **Canny Edge Detector** to extract edges before applying HT  

- 📊 **Hough Space Representation**
  - Each point in image space maps to a sinusoidal curve in parameter space  

- 🗳️ **Accumulator Array**
  - Votes are collected for possible lines  
  - Peaks represent detected lines  

- 📏 **Parameters**
  - ρ (rho): Distance from origin  
  - θ (theta): Angle of the line  

---

## ⚙️ Methodology

1. Load input image  
2. Apply **Canny Edge Detection**  
3. Transform edge points into Hough space  
4. Accumulate votes in (ρ, θ) parameter space  
5. Detect peaks in accumulator  
6. Draw detected lines on original image  

---

## ▶️ Run the Project

Run the following command:

```bash
pip install opencv-python numpy matplotlib && python hough_transform.py
