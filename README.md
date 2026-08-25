Brain_Tumor_Image_Classification

## 📌 Project Overview

Developed a deep learning model to classify brain MRI images into **Tumorous** and **Non-Tumorous** categories using **VGG19 Transfer Learning**. The project combines OpenCV-based image preprocessing, data augmentation, transfer learning, and fine-tuning to improve classification performance.

## 🎯 Objective

To develop an automated image classification system capable of distinguishing between **tumorous** and **non-tumorous** brain MRI images.

## 🛠️ Technologies Used

* Python
* TensorFlow & Keras
* VGG19
* OpenCV
* NumPy & Pandas
* Matplotlib & Seaborn
* Scikit-learn

## 🔄 Project Workflow

**MRI Dataset → Image Preprocessing → Brain Region Cropping → Data Augmentation → Dataset Split → VGG19 Transfer Learning → Fine-Tuning → Evaluation → Classification**

## 🔍 Image Preprocessing

MRI images were processed using OpenCV through:

* Grayscale conversion
* Gaussian blurring
* Thresholding
* Morphological operations
* Contour detection
* Brain-region extraction
* Image resizing and pixel normalization

## 🔄 Data Augmentation

Training images were augmented using:

* Rotation
* Width and height shifting
* Shearing
* Brightness adjustment
* Horizontal flipping
* Vertical flipping

These transformations help increase training-data diversity and improve model generalization.

## 🤖 Model Architecture

A pre-trained **VGG19 model with ImageNet weights** was used as the feature extractor.

**VGG19 → Flatten → Dense → Dropout → Dense → Softmax → 2 Classes**

## 🎓 Transfer Learning & Fine-Tuning

Three training approaches were explored:

**1. 🔒 Frozen VGG19**
The VGG19 base layers were frozen while the custom classification layers were trained.

**2. 🔧 Incremental Fine-Tuning**
Selected VGG19 layers were gradually unfrozen and retrained to adapt the model to brain MRI images.

**3. ⚙️ Full Network Training**
The complete VGG19 network was unfrozen for further model adaptation.

## 📊 Model Evaluation

Model performance was analyzed using:

* Training accuracy
* Validation accuracy
* Training and validation loss
* Testing accuracy
* Testing loss
* Accuracy and loss curves

## ⭐ Key Highlights

* Built a deep learning pipeline for brain MRI classification.
* Applied OpenCV techniques for image preprocessing.
* Implemented VGG19 transfer learning.
* Used data augmentation to improve generalization.
* Explored multiple fine-tuning strategies.
* Evaluated performance using training, validation, and testing datasets.

