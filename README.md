# Rice Leaf Disease Detection & Classification
This project aims to build a deep learning pipeline for the early detection and classification of three major rice leaf diseases: Leaf Smut, Brown Spot, and Bacterial Leaf Blight. By leveraging image data and advanced modeling techniques, this solution supports smarter agricultural interventions and improved crop yield.

# Objective
To automate the identification of rice leaf diseases using image classification techniques, thereby aiding farmers and agronomists in timely diagnosis and management.

# Dataset
Total Images: 120 leaf images

Classes:

Leaf Smut

Brown Spot

Bacterial Leaf Blight

Image Size: Resized to 224x224 pixels for model compatibility

Data Split: 95 training, 12 validation, 12 testing samples

> Note: Dataset is proprietary and is not included in this repository. Please contact the author for access.

# Technologies & Libraries
Python, NumPy, Matplotlib, Scikit-learn

TensorFlow / Keras (CNN, Data Augmentation, Transfer Learning)

Pretrained Model: VGG16 (for transfer learning)

ImageDataGenerator for real-time image augmentation

# Approach
🔹 Phase 1: Baseline CNN
Achieved ~50% test accuracy

Identified signs of overfitting and poor generalization

🔹 Phase 2: Data Augmentation
Techniques: rotation, zoom, flip, shift, shear

Accuracy dropped to ~41.6% indicating suboptimal learning

🔹 Phase 3: Transfer Learning (VGG16)
Frozen base layers + custom classifier head

Final test accuracy: 91.67%

Demonstrated robustness and superior generalization

# Training Performance
Model Type	Test Accuracy
Baseline CNN	50.00%
CNN + Data Augmentation	41.67%
Transfer Learning (VGG16)	91.67%
> 📊 Transfer learning proved to be the most effective strategy for this task.

# Evaluation & Visualization
Plots for accuracy and loss (training vs. validation)

Overfitting spotted in early models

Data augmentation improved robustness marginally

Transfer learning yielded stable, high-accuracy performance

# Future Scope
Collect and label more images for better generalization

Fine-tune deeper layers of pretrained models

Experiment with other architectures (ResNet, Inception)

Deploy as a web or mobile app for field use
