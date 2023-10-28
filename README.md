# Brain-Tumor-Detection

# Brain Tumor Detection 🧠

![brain_Mri](https://github.com/krishnah1/Brain_Tumor_Detection/assets/65085409/2bd6457b-eb0b-42b6-8255-ac85af2c90e4)


**Brain tumor detection** is the use of medical imaging methods to identify and evaluate the presence and specific characteristics of brain tumors, contributing to the diagnosis and treatment planning process in the field of medicine.

## 📃Table of Contents

- [Motivation](#-motivation)
- [Tech Stack](#%EF%B8%8Ftech-stack)
- [Features](#-features)
- [Data Sets](#-data-sets)
- [Data Augmentation](#data-augmentation)
- [Data Preprocessing](#-data-preprocessing)
- [Data Split](#data-split)
- [Results](#-results)
  
## 😇 Motivation

A brain tumor is a mass or growth of abnormal cells in your brain. There are many types of brain tumors that doctors take a lot of time to find and analyze. This decreases the efficiency of the treatment and is a sheer waste of time. Using the segmentation concept, the tumor can be found within
no time and with much more efficiency. This thesis presents a novel, fully automatic method for intracranial boundary detection and intensity correction in MR images of the head. The intracranial boundary is the boundary between the brain and the intracranial cavity. It accurately segments the brain from other features in the head.
## ⚠️Tech Stack

- **Support Vector Machine (SVM)**

- **Keras**

- **TensorFlow** 

- **Scikit learn** 

- **Matplotlib** 


## ⭐ Features

- The system accurately localizes and identifies the presence of brain tumors within MRI.

-  It categorizes tumors into relevant types, such as benign or malignant, and provides detailed information about their size, shape, and other attributes, aiding in treatment planning.

- Users can fine-tune the system by adjusting model settings and parameters to optimize its performance in various clinical scenarios and environmental conditions.
## 📂 Data Sets
- The data sets can be [downloaded here](https://www.kaggle.com/datasets/navoneel/brain-mri-images-for-brain-tumor-detection)

- The dataset is organized into two primary folders: **"yes"** and **"no"**, collectively containing **253** Brain MRI Images. 
- Within the **"yes"** directory are **155** Brain MRI Images illustrating tumorous cases. 
- within the **"no"** directory houses **98** Brain MRI Images showcasing non-tumorous instances.

## 🌱Data Augmentation

- Due to the dataset's limited size, there were insufficient instances for robust neural network training. Data augmentation proved valuable in addressing the data imbalance problem within the dataset.

- Before data augmentation, the dataset consisted of: **155 positive** and **98 negative** examples, resulting in **253** example images.

- After data augmentation, now the dataset consists of: **1085 positive** and **980 negative** examples, resulting in **2065** example images. 

**NOTE** : The dataset of **2065** examples includes the original **253** images, all of which can be found within the **'augmented_data'** folder.





## 🔃 Data Preprocessing 

For each image, the subsequent preprocessing procedures were implemented:

- The image was cropped to retain only the brain region, as it constitutes the most vital component of the image.
- The image was resized to adopt a standardized format of **(240, 240, 3)**, which encompasses the dimensions of image width, height, and number of channels. This uniformity was necessary as the dataset contained images of varying sizes to ensure compatibility for neural network input.
- Normalization was applied to rescale pixel values, confining them within the **0-1 range**. This process was crucial for consistency and improved neural network performance.
## 🪓Data Split

The data partitioning was carried out as follows:

- **70%** of the data was allocated for **training** purposes.
- **15%** of the data was designated for **validation**.
- Remaining **15%** of the data was set aside for **testing**.
## 🔑 Results
The results for Brain Tumor Detection are 

- **88.7%** accuracy on Test Set. 

- **0.88** f1 score on the Test Set for Brain Tumor Detection.

- **91%** accuracy on Validation Set

- **0.91** f1 score on the Validation Set for Brain Tumor Detection
