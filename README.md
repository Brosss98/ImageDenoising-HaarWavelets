# Image Denoising using Haar Wavelets

Author: **Mario Medone**  
Course: *Digital Signal & Image Processing*

---

## 📖 Project Overview
This repository contains an implementation of **image denoising using Haar wavelets**.  
Wavelet-based denoising is a powerful technique for reducing noise in digital images, 
particularly Gaussian noise, while preserving important structural details.

The project explores:
- The application of the **Haar wavelet transform** for image decomposition.
- The role of **hard and soft thresholding** in noise removal.
- The challenge of selecting an appropriate threshold parameter.
- The use of **BayesShrink** as a standard method for threshold estimation.

---

## ⚙️ Methodology
1. **Introduction**
    We introduce the concept of digital images and the presence of noise, focusing 
    particularly on Gaussian noise. We highlight its statistical properties and 
    emphasize the independence of Gaussian noise with respect to the 2D wavelet 
    transform.
2. **Literature Review**
    This section provides a brief overview of the 2D Haar wavelet transform, the 
    denoising procedure, and the different wavelet thresholding methods. A detailed 
    discussion is included on the challenges of selecting the optimal threshold 
    parameter, supported by insights from previous works.
3. **Implementation**
    We implement the thresholding methods and the denoising procedure described in the 
    literature, applying them to test images in order to evaluate their effectiveness.
4. **Experimental Results**
    The implemented methods are tested and compared. Based on the outcomes, we analyze 
    which thresholding approach and parameter selection strategy yield the most 
    effective denoising performance.
5. **Conclusions**
    We summarize the findings and provide final considerations on the overall work, 
    highlighting the strengths and limitations of Haar wavelet-based denoising.

---

## 📊 Results & Conclusions
- Haar wavelets are a **useful and powerful tool** for clearing images from noise, 
especially Gaussian noise.  
- The choice of threshold parameter is **non-trivial**; standard methods like 
BayesShrink help automate this process.  
- The **best configuration** observed:
    - Apply **soft thresholding** to detail coefficients.
    - Use **BayesShrink** for threshold definition.
- Denoised images show **good quality**, though performance decreases as noise 
increases:
    - Higher Gaussian noise standard deviation leads to grainier and blurrier results.

---

## 🚀 How to Run
1. Clone the repository:
    ```bash
    git clone https://github.com/Brosss98/ImageDenoising-HaarWavelets.git
    cd ImageDenoising-HaarWavelets
    ```
2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```
3. Run the notebook

---

## 📚 References
A list of the articles, works, and projects consulted to understand Haar wavelet-based 
image denoising and to build this laboratory:

1. Yang Qiang, *Image denoising based on Haar wavelet transform*.  
   Proceedings of the 2011 International Conference on Electronics and Optoelectronics, 
   2011, pp. V3-129–V3-132.  
   doi: [10.1109/ICEOE.2011.6013318](https://doi.org/10.1109/ICEOE.2011.6013318)

2. J. Pang, *Improved image denoising based on Haar wavelet transform*.  
   2017 IEEE SmartWorld, Ubiquitous Intelligence & Computing, Advanced & Trusted 
   Computing, Scalable Computing & Communications, Cloud & Big Data Computing, Internet 
   of People and Smart City Innovation (SmartWorld/SCALCOM/UIC/ATC/CBDCom/IOP/SCI), 
   2017, pp. 1–6.  
   doi: [10.1109/UIC-ATC.2017.8397456](https://doi.org/10.1109/UIC-ATC.2017.8397456)

3. S. H. Ismael, F. M. Mustafa, I. T. Okümüs, *A New Approach of Image Denoising Based 
on Discrete Wavelet Transform*.  
   2016 World Symposium on Computer Applications & Research (WSCAR), 2016, pp. 36–40.  
   doi: [10.1109/WSCAR.2016.30](https://doi.org/10.1109/WSCAR.2016.30)

4. Shivani Mupparaju, B. Naga Venkata Satya Durga Jahnavi, *Comparison of Various 
Thresholding Techniques of Image Denoising*.  
   Department of ECE, VNR VJIET, Hyderabad, A.P, India. International Journal of 
   Engineering Research & Technology (IJERT), Vol. 2 Issue 9, September 2013.  
   ISSN: 2278-0181

5. Gregory R. Lee, Ralf Gommers, Filip Wasilewski, Kai Wohlfahrt, Aaron O’Leary, 
*PyWavelets: A Python package for wavelet analysis*.  
   Journal of Open Source Software, 4(36), 1237, 2019.  
   doi: [10.21105/joss.01237](https://doi.org/10.21105/joss.01237)