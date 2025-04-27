# Image_Manipulation_and_Data_Augmentation-Python

This repository contains a Python-based homework assignment for practicing **NumPy array manipulation** techniques, using **image processing** tasks on `.jpg` and `.png` files. The objective was to strengthen fundamental array skills while also introducing core concepts of **data augmentation** for machine learning using image transformations.

---

### 🧩 Business Problem

In real-world machine learning projects, data is often limited. To train better models without collecting more data, **data augmentation** is used — especially in computer vision tasks. Augmenting the data helps prevent **overfitting** and improves **model generalization** by artificially expanding the dataset using transformations like flipping, color manipulation, cropping, and gamma correction.

This assignment explores how simple NumPy operations can simulate real-world data augmentation processes on images, an essential skill for data scientists and AI engineers.

---

### 📦 Dataset Overview

The images used were provided in two formats:

- `img1.jpg` – RGB color image
- `img1.png` – RGBA color image (with an Alpha transparency channel)

Both images depict the same scene but differ slightly in data storage structure and pixel value scaling (`0-255` for JPG and `0.0-1.0` for PNG).

---

### 🎯 Project Objective

This assignment focused on:

- Importing and reading images into NumPy arrays
- Visualizing images with **Matplotlib**
- Exploring image structures (dimensions, pixel values, datatypes)
- Practicing NumPy indexing, slicing, and broadcasting
- Performing **data augmentation** tasks including:
  - Image flipping (horizontal and vertical)
  - Transparency manipulation
  - Color inversion (negative images)
  - Image cropping
  - Grayscale conversion
  - Gamma correction for brightness adjustment
  - Color-channel isolations (Red, Green, Blue scales)
  - Horizontal stacking of color-isolated images

All tasks were completed using only **NumPy** and **Matplotlib** — no external image processing libraries like OpenCV or PIL were used.

---

### 🛠️ Solution Approach

The complete workflow involved:

**1. Housekeeping:**
- Notebook documentation with name and proper section headings.

**2. Image Import and Display:**
- Used `matplotlib.pyplot.imread()` to read `.jpg` and `.png` images.
- Created a reusable `display_image()` function to visualize images with axis labels and colorbars.

**3. Image Structure Exploration:**
- Examined object types, shapes, pixel counts, and datatype differences between PNG and JPG formats.

**4. Data Augmentation via Array Manipulations:**
- **Horizontal and vertical flips** via array slicing and `np.flip()`
- **Transparency adjustment** on specific sections of the image
- **Negative transformations** by inverting RGB channels
- **Cropping** selected image regions
- **Converting to grayscale** using weighted averages of RGB channels
- **Gamma correction** for brightness modification
- **Color isolation and stacking** into a combined visualization

---

### 💡 Business Value

This assignment mirrors real-world needs in:

- **Deep Learning**: Preparing augmented datasets for CNNs or vision models
- **Data Science**: Image-based feature engineering
- **Computer Vision**: Manipulating images for tasks like object detection, segmentation, and classification

The ability to perform low-level array-based image manipulation builds essential intuition and coding skills required for advanced work with images and video data.

---

### 🚧 Challenges Encountered

- **Data scaling differences** between PNG and JPG formats required attention to color value ranges
- **Transparency manipulation** involved careful slicing and updating only the Alpha channel
- **Maintaining original images** when creating transformations to avoid overwriting
- **Handling axis dimensions correctly** during flips and stacking operations

---

