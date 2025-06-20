A comprehensive machine learning pipeline for automated identification and classification of retinal neuronal subtypes using DAPI-stained microscopic images.
All image data were taken from the Vision Biology Lab at IIT Madras, headed by Prof. Santosh Sethuramanujam. 

## Project Overview
This project implements an end-to-end pipeline for classifying retinal cells into distinct neuronal subtypes using nuclear morphology and spatial distribution patterns (the code for this is coming soon! ).
The system achieves 99.28% test accuracy in distinguishing between photoreceptors and other retinal cell types.

Key Features
1. Automated Cell Segmentation: Cellpose-based nuclear segmentation
2. Multi-class Classification: Support for photoreceptors, rod bipolar cells, cone bipolar cells, and other cell types
3. High Performance: VGG16-based CNN with transfer learning
4. Scalable Pipeline: Modular design for processing large datasets
5. Comprehensive Analysis: Including IoU-based overlap analysis for marker validation

Code Files Involved: 
Cell Extraction
* Retinal_Cell_Extract_PRs.ipynb          # Photoreceptor extraction
* Retinal_Cell_Extract_oth.ipynb          # Other cell extraction
* extract_SCGNs_cbc.ipynb                 # Cone bipolar cell extraction
* extract_pkc_rbc.ipynb                   # Rod bipolar cell extraction
Data_processing
* retina_classification_size_label_sort.ipynb  # Data preprocessing
* retinal_cell_avging.ipynb               # Cell averaging analysis
Model_training
* Retina_classification_retrain_VGG16.ipynb   # Model training
* Retina_Classification_load_deploy_best_model.ipynb  # Model deployment
