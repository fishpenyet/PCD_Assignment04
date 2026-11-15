# PCD Assignment — Image Processing Case Studies (IEEE Report)
 
**Name:** Naila Syakira
**NIM:** 25/555286/PA/23270
 
This repository contains a short IEEE-format report that summarizes three published articles showing how digital image processing solves real problems, and identifies which image features suit each case. The cases are listed below.
 
## Case Studies & Suitable Features
 
* **Low-Contrast Chest X-Ray** — Hatipoğlu et al. (2022). CLAHE applied only to low-contrast images before a pneumonia/COVID-19 classifier. Suitable features: gray-level histogram, overall contrast
* **Noise Removal in Medical Images** — Boby & Sharmin (2021). Mean, median, Gaussian (and other) filters on ultrasound, CT, and MRI images. Suitable feature: local pixel neighborhood
* **Lane Line Detection** — Javeed et al. (2023). Gaussian blur, Otsu threshold, Sobel/Canny edges, and fast Hough transform. Suitable features: intensity, edges, straight lines
## Files
 
* `IEEE_Report_Three_Image_Processing_Cases.docx` — the report
## Notes
 
This is a summary report only. No experiments were rerun, so all numbers come from the three articles, and the figures were redrawn from the tables in those articles. Main findings: selective CLAHE raised classifier accuracy from 95.22% to 97.35%; the median filter was best for salt-and-pepper noise (32.1 dB PSNR) while the Gaussian filter was best for speckle noise (25.7 dB); and the lane detector reached 89.5%–96.7% accuracy at about 20–22 ms per frame. The main lesson is that the best feature depends on the problem: the histogram for contrast, the pixel neighborhood for noise, and edges and lines for shape.
 
