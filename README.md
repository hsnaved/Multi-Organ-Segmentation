# Multi-Organ-Segmentation
**Overview**

This project involves creating a mobile application for multi-organ segmentation in abdominal CT images using advanced deep learning architectures, including the UNETR model, which combines Vision Transformers and CNNs for enhanced segmentation accuracy. The application allows users to segment organs and visualize segmentation results on a mobile interface, integrating deep learning algorithms with a user-friendly app.

NOTE: I have worked on dataset and model developing

# 🎯Objectives

- Develop a mobile app for multi-organ segmentation in abdominal CT images.
- Implement a Transformer-based architecture (UNETR) for precise segmentation.
- Integrate model functionality into a mobile app using Flutter.
- Deploy the segmentation model on cloud infrastructure for accessible and efficient inference.

# 🛠️Technology Stack
- Mobile Front-end: Flutter
- Authentication: Google Firebase
- Deep Learning Framework: TensorFlow
- Data Processing: NumPy, OpenCV
- Deployment: Amazon Web Services (AWS)
- Hardware: Utilized CPU, GPU, and TPU for model training to optimize performance.

# 📊Dataset
- Name: Synapse Multi-Organ Segmentation Dataset
- Source: Multi-Atlas Labeling Beyond the Cranial Vault - Synapse
- Description: Contains 30 abdominal CT scans with 3779 contrast-enhanced clinical CT images, focusing on 10 organs plus a background class.
- Data Usage: For this project, 2 folders (4720 images and masks) were used, with manual conversion of greyscale values to color images for better organ differentiation.
  
# 🏗️Model Architecture
**UNETR
- Combines Vision Transformers for context and CNNs for localization.
- Encoder: Transforms input images into feature maps using Transformer layers with attention mechanisms.
- Decoder: Upsamples and refines segmentation, achieving high spatial resolution with skip connections.
- Output: A 1x1 convolution layer with Softmax activation provides class probabilities for each pixel.

# 🎓Training and Performance
-Hardware and Platforms
- CPU Training: Local 4-core CPU (16GB RAM); slow, with each epoch taking over 6 hours.
- GPU Training:
- Google Colab (T4 GPU): Batch sizes 4-6, epochs up to 100.
- Kaggle (32GB GPU): Batch size 8, epoch ETA ~200 seconds.
- TPU Training: Google Cloud TPU (128GB memory) enabling batch sizes up to 32, reducing epoch ETA to ~60 seconds.
**Performance Metrics
- Dice Score and Intersection over Union (IoU) were used to evaluate model performance across different organ classes.
  
# 💡Applications
Multi-organ segmentation has critical applications in medical imaging, aiding in precise diagnosis, surgical planning, and treatment monitoring. Key uses include:

- Disease Diagnosis: Enables detailed analysis of organs, helping identify conditions like tumors, liver cirrhosis, and kidney diseases.

- Surgical Planning: Assists surgeons in visualizing organ structures for safer, more effective surgeries.

- Radiation Therapy: Supports accurate targeting of radiation doses, minimizing damage to surrounding healthy organs.

- Medical Research: Facilitates anatomical studies and data collection for new treatments and medical advancements.

This technology streamlines clinical workflows and improves patient outcomes through enhanced organ visualization and analysis.
