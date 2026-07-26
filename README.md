#  Flood Detection using SAR Images with Attention U-Net

A deep learning project for automatic flood detection from **Synthetic Aperture Radar (SAR)** imagery using an **Attention U-Net** architecture with a **ResNet34 encoder**.

The model is designed to accurately segment flood-affected regions from SAR images while reducing the impact of speckle noise using **Lee Filtering**. It also incorporates **Grad-CAM** to improve model interpretability by highlighting the image regions that influence predictions.

This project was developed during my internship at the **Maharashtra Remote Sensing Applications Centre (MRSAC), Nagpur**.

---

#  Project Overview

Floods are among the most devastating natural disasters, requiring timely and accurate detection for effective disaster response.

Unlike optical satellite imagery, **Synthetic Aperture Radar (SAR)** can capture Earth's surface regardless of cloud cover or lighting conditions, making it ideal for flood monitoring.

This project leverages deep learning to automatically identify flooded regions from SAR imagery through semantic segmentation.

---

#  Features

- Flood segmentation using SAR images
- Attention U-Net architecture
- Pretrained ResNet34 encoder
- Lee Filter for SAR speckle noise reduction
- Dice + BCE hybrid loss
- Data augmentation
- Dice Score & IoU evaluation
- Grad-CAM visualization
- Automatic prediction saving
- Model checkpointing

---

#  Technologies Used

- Python
- PyTorch
- Torchvision
- OpenCV
- NumPy
- Matplotlib
- PIL
- Scikit-Learn
- Kaggle
- Google Colab / Jupyter Notebook

---

# Model Architecture

```
SAR Image
     │
Lee Filter
     │
Data Augmentation
     │
Attention U-Net
(ResNet34 Encoder)
     │
Flood Segmentation Mask
     │
Performance Evaluation
(Dice Score & IoU)
     │
Grad-CAM Visualization
```

---

# ⚙️ Workflow

1. Load SAR image dataset.
2. Apply Lee Filter to reduce speckle noise.
3. Resize and augment images.
4. Train Attention U-Net with a pretrained ResNet34 encoder.
5. Optimize using Dice + BCE Loss.
6. Evaluate model using Dice Score and IoU.
7. Generate flood segmentation masks.
8. Visualize model attention using Grad-CAM.
9. Save trained model and prediction outputs.

---

#  Evaluation Metrics

The model is evaluated using:

- Dice Score
- Intersection over Union (IoU)
- Binary Cross Entropy (BCE) Loss
- Dice Loss

---

#  Project Structure

```
SAR-Flood-Detection/
│
├── SAR_Flood_Detection_Attention_UNet.ipynb
├── dataset/
├── checkpoints/
├── predictions/
├── gradcam/
├── README.md
└── requirements.txt
```


#  Key Highlights

- Attention U-Net improves segmentation by focusing on important spatial regions.
- ResNet34 encoder enhances feature extraction through transfer learning.
- Lee Filtering minimizes SAR-specific speckle noise before model training.
- Grad-CAM provides explainable AI by visualizing model attention.
- Hybrid Dice + BCE Loss improves segmentation performance.

---

#  Applications

- Flood Monitoring
- Disaster Management
- Emergency Response
- Remote Sensing
- Environmental Monitoring
- Geospatial Intelligence



#  Future Improvements

- Multi-temporal SAR analysis
- Real-time flood detection
- Cloud deployment
- Transformer-based segmentation models
- Multi-class disaster segmentation
- GIS integration


#  Learning Outcomes

Through this project, I gained practical experience in:

- Deep Learning
- Computer Vision
- Semantic Segmentation
- Attention U-Net
- Transfer Learning
- ResNet34
- Explainable AI (Grad-CAM)
- SAR Image Processing
- PyTorch
- Remote Sensing
