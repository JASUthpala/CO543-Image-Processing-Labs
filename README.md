# Image Processing Lab Notebooks - CO543 (2025)

**Department of Computer Engineering, University of Peradeniya**  
**Course:** CO543 - Image Processing  
**Labs** 
**Author:** Sandali Uthpala  

This repository contains my **Image Processing laboratory work** implemented in **Jupyter Notebooks**. The notebooks cover hands-on exercises exploring fundamental image processing concepts, pixel-space operations, and illumination/contrast adjustments using Python and OpenCV.

---

## Lab 1: Seeing Images as Numbers and Understanding Basic Transformations
- Visualizing images as numeric arrays  
- Grayscale conversion and structure inspection  
- Image resizing and zoom to study resolution effects  
- Cropping, flipping, and rotation transformations  
- Pixel intensity inversion (negative images)  
- Converting CSV digit data to images  
- Simple affine transformations  
**Focus:** Understanding how computers represent and manipulate images at the pixel level.

---

## Lab 2: Illumination, Contrast and Thresholding Fundamentals
- Visualizing intensity distributions & histograms  
- Manual thresholding and failure cases  
- Otsu and adaptive thresholding  
- Gamma correction & log transformations  
- Contrast stretching & histogram equalization  
- Bit-plane slicing  
**Focus:** Enhancing and normalizing images under varying lighting conditions, and understanding the effect of intensity transformations on perception and segmentation.

---


## Lab 3: Noise Removal and Structure Preservation
- Simulation of salt-and-pepper noise on clean facial images  
- Analysis of how random noise disrupts fine structures and visual continuity 
- Noise reduction using mean (average) filtering and discussion on blur-induced detail loss
- Median filtering for effective removal of impulse noise while preserving edges
- Gaussian smoothing and analysis of noise–detail trade-offs
- Bilateral filtering for edge-aware noise reduction
- Laplacian-based sharpening to enhance structural boundaries
- Study of how sharpening can re-amplify noise if applied excessively

**Focus:** Understanding the balance between denoising and detail retention, and evaluating classical spatial-domain filters based on their ability to suppress noise while preserving edges and facial identity.

---

## Lab 4: Segmentation and Image Restoration 
- Foreground–background separation using global thresholding
- Adaptive thresholding for handling uneven lighting
- Analysis of limitations of intensity-based segmentation
- K-means clustering for pixel grouping based on intensity
- Isolation of scribbles/damaged regions using clustering
- Edge detection using Canny to identify structural boundaries
- Comparison of scene structure edges vs scribble edges
- Creation of masks for damaged areas
- Image restoration using Telea inpainting
- Evaluation of blending quality and visual realism
- Discussion on limitations of inpainting on complex textures

**Focus:** Applying segmentation techniques to support realistic image restoration while preserving important structural details.

--- 

## Lab 5: Edges, Corners and Structural Features 
- Edge detection using Sobel operator (first-order gradients)
- Edge detection using Laplacian operator (second-order derivatives)
- Comparison of directional sensitivity (Sobel) vs double-edge response (Laplacian)
- Analysis of edge smoothness and noise sensitivity
- Canny edge detection for thin and clean binary edge maps
- Study of threshold selection and hysteresis for noise suppression
- Corner detection using Shi-Tomasi / Harris method
- Identification of stable and distinctive feature points
- Discussion on why corners are useful for matching and tracking
- Line detection using Hough Transform on Canny edges
- Extraction of dominant straight lines in man-made structures
- Analysis of vote threshold effects on line detection results

**Focus:** Understanding how edges, corners, and lines represent structural geometry in images, and how these features form the foundation for mapping, stitching, tracking, and object recognition systems.

--- 

## Lab 6: Unsupervised and Supervised Digit Recognition
- Loading digit dataset from CSV and reshaping 784-length vectors into 28×28 images
- Visualization of sample handwritten digits in grayscale
- Analysis of why correct reshaping is essential for meaningful image representation
- Unsupervised clustering of digits using K-Means (k = 10)
- Visualization of clustered samples and comparison of cluster purity
- Discussion on why visually similar digits (e.g., 3, 5, 8) group together
- Training a simple MLP classifier using flattened pixel inputs
- Evaluation using test accuracy and confusion matrix
- Analysis of limitations of treating pixels as independent features
- Training a CNN with convolution, activation, pooling, and dense layers
- Comparison of CNN performance with MLP and K-Means clustering
- Explanation of how CNNs exploit local spatial structure and translation invariance
- Inspection and analysis of misclassified digits across models
- Comparison of failures in clustering, MLP, and CNN approaches

**Focus:** Understanding the progression from unsupervised clustering to supervised classification, and analyzing how data representation and model architecture influence digit recognition performance.

--- 

## Lab 7: Transfer Learning and Fine-Tuning 
- Loading a pretrained CNN model (e.g., ResNet18)
- Replacing the final classification layer for a custom dataset
- Freezing early layers to use the network as a fixed feature extractor
- Training only the new classifier layer and reporting training/validation accuracy
- Analysis of how pretrained layers act as generic feature detectors
- Unfreezing the last convolutional block for partial fine-tuning
- Training with a smaller learning rate to refine higher-level features
- Comparison of convergence speed and overfitting behavior
- Evaluation of performance differences between frozen and fine-tuned models
- Discussion on when fixed-feature extraction is sufficient
- Analysis of when domain shift requires fine-tuning
- Examination of overfitting risks on small datasets during fine-tuning

**Focus:** Understanding how transfer learning leverages pretrained representations to reduce training time and data requirements, and analyzing when partial fine-tuning improves performance over fixed feature extraction.

---

## Lab 8: Frequency-Domain Filtering for Artifact Removal
- Visualizing the frequency spectrum using 2D FFT
- Shifting zero-frequency component to the center
- Observing low-frequency and high-frequency components
- Identifying periodic noise patterns in the spectrum
- Designing a circular low-pass frequency mask
- Filtering high-frequency components in the frequency domain
- Reconstructing the image using inverse FFT
- Comparing original and filtered images
- Analyzing blurring effects due to high-frequency removal
- Understanding when frequency filtering is preferable over spatial filtering

**Focus:** Understanding how images can be analyzed and cleaned in the frequency domain, especially for removing structured or periodic noise.

---

## Tools & Technologies
- **Python 3**  
- **Jupyter Notebook** (.ipynb)  
- **OpenCV, NumPy, Matplotlib**  

---

## Notes
These notebooks are intended for educational purposes to demonstrate image processing concepts learned during the CO543 labs.

