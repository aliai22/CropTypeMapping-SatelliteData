
# Crop Type Mapping Using Transfer Learning

This repository contains the implementation of a transfer learning-based approach for crop type mapping using Sentinel-2 imagery. The project involves training a U-Net segmentation model (pretrained on ImageNet with InceptionResNetV2 backbone) on CORINE land cover data for rice crop classification. The trained model was applied to a local region (Sargodha, Pakistan) for predicting rice field locations using manually prepared labels based on vegetation indices like NDVI.

## Project Overview

- **Objective:** Use satellite imagery and deep learning for automated crop type mapping to produce moderately accurate crop maps in label scarced regions as a starting point.
- **Datasets:**
    - ***Training:*** Rice crop maps extracted from *CORINE* land cover data.
    - ***Application:*** Sentinel-2 imagery of rice fields in Sargodha region, manually labeled using NDVI.
- **Methods:**
    - U-Net architecture with *InceptionResNetV2* backbone.
    - Transfer learning for semantic segmentation.
- **Results:**
    - Moderately accurate rice crop maps.
    - Visual comparison of predicted masks and ground truth labels.

## 🛠️ Installation

To replicate this project, follow these steps:

1. Clone the repository:
    `git clone https://github.com/aliai22/CropTypeMapping-SatelliteData.git`

2. Install required dependencies:
    `pip install -r requirements.txt`

## 📊 Key Results
Below are some sample outputs:

- **Training:**

![training_results](https://github.com/user-attachments/assets/84a023da-b574-4658-ac2e-5b048809ec4d)


- **Testing:**

![testing_results](https://github.com/user-attachments/assets/1bb7cf3d-4be6-49d7-8df7-f20e5fdec8bd)


## 🔍 Model Details

- Architecture: U-Net with InceptionResNetV2 backbone.
- Pretraining: ImageNet weights for feature extration.
- Metrics: IoU, Jaccard Coefficient, Precison, and Recall.

## 💡 Future Work

- Expand the methodology to other crops and regions.
- Automate label generation using AI-based vegetation index analysis.

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to fork the repository and submit a pull request.
