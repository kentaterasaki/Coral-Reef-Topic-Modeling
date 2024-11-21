# Coral Reef Topic Modeling with SAM

## Overview

Surveying coral reefs is traditionally a manual, labor-intensive process conducted by divers. This limits the frequency and breadth of data collection, leaving gaps during critical environmental events such as heatwaves or hurricanes. To address this challenge, we partner with the University of Puerto Rico to deploy low-cost surface vessels equipped with camera systems to map reefs visually.

This repository focuses on one branch of the project: **automatic coral reef topic modeling**. We implement **Segment Anything Model (SAM)** and clustering techniques (using **K-Means clustering**) to segment and analyze images of coral reefs. By clustering extracted features, we derive topics representing different coral reef landscapes, offering insights into their structure and health.

---

## Features of This Repository

1. **Coral Reef Image Preprocessing**
   - Enhances images using color normalization.

2. **Coral Segmentation with SAM**
   - Generates segmentation masks for reef regions using the Segment Anything Model (SAM).
   - Custom algorithm removes overlapping masks and applies size thresholds.

3. **Feature Extraction**
   - Extracts advanced features (e.g., CNN features, color, and texture metrics) for each segmentation mask.
   - Supports models like ResNet-18 for feature extraction.

4. **Topic Modeling**
   - Utilizes **K-Means clustering** to derive topics representing different coral reef structures.
   - Automatically selects the optimal number of topics using silhouette analysis.

5. **Visualizations**
   - Generates mask overlays and topic distributions for individual images and global datasets.
   - Uses bar plots and heatmaps to visualize topic contributions across the dataset.

![filter1](https://github.com/user-attachments/assets/920039ac-a7b3-4f39-8794-92e461fefeac)
![filter2](https://github.com/user-attachments/assets/bdc52e83-fc7d-41c1-b4dd-f545dff28e71)

