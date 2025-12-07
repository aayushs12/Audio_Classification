# Urban Sound Classification using Deep Learning

##Repository Structure
This project is organized into three distinct notebooks, representing the progression from data analysis to advanced model implementation:
1. **EDA_Audio_Classification.ipynb**
Phase: Exploratory Data Analysis & Visualization
Data Setup: Handles the automatic downloading and validation of the UrbanSound8K dataset using the soundata library .
Distribution Analysis: Visualizes class imbalances and fold distributions to understand the dataset structure .
Feature Visualization: Generates plots for Waveforms, Mel-Spectrograms, and MFCCs to visually compare different sound categories .

2. **Audio_Classification_Models.ipynb**
Phase: Machine Learning, Custom Deep Learning & Transfer Learning
Feature Engineering: Implements caching for extracting MFCC statistics (for ML) and Mel-Spectrograms (for DL) .
Traditional ML: Trains and evaluates baseline models including Random Forest, Support Vector Classifier (SVC), and K-Nearest Neighbors (KNN) .
Deep Learning: Implements custom architectures including Artificial Neural Networks (ANN), 1D CNNs, and 2D CNNs .
Transfer Learning: Fine-tunes an EfficientNet-B0 model modified for single-channel audio, utilizing MixUp augmentation to improve performance .

3. **AST.ipynb**
Phase: Transformer
Model Implementation: Fine-tunes the Audio Spectrogram Transformer (AST) (specifically MIT/ast-finetuned-audioset) .
Preprocessing: Handles specific AST requirements, including resampling to 16kHz and padding inputs to 1024 frames .
Evaluation: Achieves the highest accuracy and produces detailed evaluation visualizations including Confusion Matrices, ROC Curves, and per-class accuracy reports .

## Project Summary

This project focuses on classifying urban environmental sounds using deep learning techniques. I will implement ML and DL models applied to mel-spectrogram representations of audio data to classify sounds into 10 distinct categories including sirens, dog barks, drilling, street music, gunshots, and more.

The model is trained and evaluated using the UrbanSound8K dataset with 10-fold cross-validation methodology. Various audio preprocessing techniques (normalization) and data augmentation strategies (pitch shifting, time stretching) will be employed to improve model robustness.

**Key Features:**
- Deep learning models built from scratch for audio classification
- Mel-spectrogram-based audio feature extraction
- 10-fold cross-validation for robust evaluation
- Audio data augmentation techniques
- Real-world applications in smart cities, public safety, and autonomous vehicles

___

**Course:** CSCI 6366 - Neural Networks and Deep Learning

**Instructor:** Professor Joel Klein

## Team Members

| Name | GitHub Username |
|------|----------------|
| Aayush Singh | [aayushs12](https://github.com/aayushs12) |

## Dataset

**UrbanSound8K Dataset**
- **Source:** [UrbanSound8K Official Website](https://urbansounddataset.weebly.com/urbansound8k.html)
- **Description:** Contains 8,732 labeled sound excerpts (≤4s) from 10 classes of urban sounds
- **Classes:** Air conditioner, car horn, children playing, dog bark, drilling, engine idling, gunshot, jackhammer, siren, street music
- **Format:** Audio files organized in 10 pre-defined folds for cross-validation

**Download Links:**
- [Dataset Download Page](https://urbansounddataset.weebly.com/urbansound8k.html)
