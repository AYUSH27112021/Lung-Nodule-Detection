# Lung Nodule Classification using Deep Learning

## Overview
Lung cancer remains a significant global health challenge, emphasizing the critical need for early detection methods. This project proposes a deep-learning solution for classifying lung nodules found in chest CT scans, potentially revolutionizing early cancer diagnosis.

## Approach
Our approach comprises three key stages:

### Preprocessing
Firstly, we employ various image processing techniques, including normalization, filtering, and thresholding, to segment the lung region from CT scans. This preprocessing step aims to isolate the lung area for subsequent analysis.

### Segmentation
Next, we introduce a modified U-Net architecture, dubbed Conv-Unet, for segmenting individual lung nodules within the preprocessed lung region. Conv-Unet is designed to extract more intricate features compared to a standard U-Net, which could lead to superior nodule segmentation results.

### Classification
Finally, Convolutional Neural Networks (CNNs) are trained to classify the segmented nodules based on the LIDC-IDRI dataset. The objective here is to categorize the nodules as either benign or malignant, thereby aiding in clinical decision-making.

## Dependencies
This project relies on the following Python libraries:
- TensorFlow/Keras
- scikit-image
- SimpleITK (optional, for medical image processing)

**Installation:**
```bash
pip install tensorflow keras scikit-image [optional] SimpleITK
```
**Note:** Specific versions of the libraries may be required depending on your project setup.

## Usage
Use the ipynb notebook [uploaded](https://github.com/AYUSH27112021/Lung-Nodule-Detection/blob/main/model%20deployment.ipynb) .

