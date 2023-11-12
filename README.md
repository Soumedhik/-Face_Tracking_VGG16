# Face Tracking Model

This repository contains code to build a custom face tracking model using TensorFlow and Keras in a single end-to-end Python file.

## Overview

The code performs the full pipeline:

- Data Collection
  - Initializes webcam
  - Captures and saves images 
  - Releases webcam
- Manual Labeling
  - Uses LabelMe for manual bounding box annotation   
- Data Augmentation
  - Albumentations for flipping, cropping, brightness/contrast
- Model Building
  - Input layer
  - VGG16 for transfer learning
  - Custom classification and regression heads
- Model Training
  - Adam optimizer
  - Custom loss functions
  - Training loop with TensorBoard logging
- Webcam Testing
  - Real-time face detection on webcam stream
  - Bounding box visualization and labeling
  

## Usage

To run the code:

1. Install requirements from `requirements.txt`
2. Update `IMAGES_PATH` and other constants
3. Run the full notebook in sequential order

The main sections are:

- Data Collection and Labeling
  - Webcam image capture
  - Manual labeling with LabelMe
- Data Augmentation
  - Albumentations augmentation  
- Model Building
  - Input layer
  - VGG16 backbone
  - Classification and regression heads
- Model Training
  - Load datasets
  - Initialize model
  - Custom loss functions
  - Model training loop
- Webcam Testing
  - Real-time detection on webcam

Thank you!
