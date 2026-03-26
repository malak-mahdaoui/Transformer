# Image Decomposition via Discrete Wavelet Transform (DWT) 
**Python | Computer Vision | Signal Processing | Wavelet Analysis**

##  Overview
This project explores the mathematical decomposition of digital images using **Discrete Wavelet Transforms (DWT)**. By applying the **Haar Wavelet**, the system decomposes an image into a multi-level hierarchy of approximation and detail coefficients. This technique is fundamental in modern image compression (like JPEG 2000), denoising, and edge detection.

##  Key Technical Features
* **Multi-Level Decomposition:** Implements a 5-level 2D-DWT using the `wavedec2` algorithm.
* **Sub-band Analysis:** Segregates images into:
    * **Approximation (A):** The low-frequency core of the image.
    * **Horizontal (H):** Isolates horizontal edges and changes.
    * **Vertical (V):** Isolates vertical edges and textures.
    * **Diagonal (D):** Captures high-frequency noise and diagonal details.
* **Selective Reconstruction:** Features a custom reconstruction engine (`waverec2`) capable of rebuilding images while zeroing out specific spatial frequencies to analyze their structural importance.
* **Dynamic Visualization:** Automated plotting of frequency coefficients and reconstruction artifacts.

##  Technical Stack
* **Language:** Python 3.x
* **Core Libraries:** * `PyWavelets (pywt)`: For advanced wavelet mathematics.
    * `Scikit-Image`: For high-quality image data and color manipulation.
    * `OpenCV`: For image matrix operations.
    * `Matplotlib`: For visual sub-band analysis.
