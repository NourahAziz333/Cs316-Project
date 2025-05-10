# Cs316-Project
AI-Powered Deforestation and Poaching Detection using Satellite Imagery and IoT Metadata.
# AI-Powered Biodiversity Protection 

This project uses AI and satellite imagery to detect deforestation and predict poaching risk in tropical ecosystems. It integrates Convolutional Neural Networks (CNNs) and metadata from simulated IoT and socio-economic sources to perform dual classification.

##  Model Overview

- **Image Input**: Satellite images from Google Earth (South American forests)
- **Metadata**: Simulated CSVs (motion detection, poverty, road distance, etc.)
- **Architecture**: ResNet18 + Fully Connected layers for metadata
- **Output**:
  1. Deforestation label
  2. Poaching risk label

## Files

- Cs316Project.ipynb: Complete notebook with model, training, testing, and visualization
- iot_data.csv: Simulated IoT metadata
- socio_data.csv: Simulated socio-economic metadata
- resnet18_deforestation.pth: Trained model weights (optional)
- README.md: Project overview and instructions

## How to Run

1. Open the notebook in [Google Colab](https://colab.research.google.com/)
2. Mount your Google Drive:
   ```python
   from google.colab import drive
   drive.mount('/content/drive')
3. The notebook automatically generates the required metadata CSVs (`iot_data.csv` and `socio_data.csv`) — no manual upload needed.
4. Simply run all cells in order to execute the full pipeline.

   
## Results
Test Accuracy: ~94%

The hybrid model outperformed image-only classifiers by incorporating environmental context

Focal Loss and class weighting significantly improved performance on the rare class (poaching)

Visual validation confirmed correct metadata-label alignment and prediction consistency


## Team Members
 Norah Alarifi (223410672)

 Areeshah Nadeem (222410835)

 Nora Almotawa (221511427)

## Conclusion
This project demonstrates how AI can be used to protect biodiversity by monitoring environmental threats. Through a hybrid model that fuses visual data and structured metadata, we created a robust tool for classifying deforestation and poaching risks. The pipeline is end-to-end, interpretable, and customizable for deployment in real-world conservation areas. All source code, results, and resources are openly shared here to support ongoing innovation in conservation technology.
