
 Overview

This project implements a face recognition system using Principal Component Analysis (PCA) for dimensionality reduction and Support Vector Machine (SVM) for classification. The system is designed to detect and recognize faces in real-time, using OpenCV for image processing and face detection, along with Scikit-learn for machine learning components.

 Features
- Face Detection: Uses OpenCV's Haar Cascade Classifier to detect faces from live video streams or images.
- Dimensionality Reduction: Applies PCA to reduce the dimensionality of the face images for more efficient processing.
- Classification: Implements a linear SVM to classify the reduced feature set and recognize faces.
- Real-time Recognition: The system can recognize faces from a live camera feed after training on a labeled dataset of faces.

 Technology Stack
- OpenCV: For face detection and image manipulation.
- Scikit-learn: Used for machine learning models including PCA and SVM.
- NumPy: For numerical computation and image data manipulation.
- Python: Primary programming language for the project.

 Workflow
1. Data Preprocessing:
   - Load and normalize face images.
   - Encode the labels using a `LabelEncoder` for classification.
   
2. PCA for Dimensionality Reduction:
   - PCA reduces the high-dimensional image data into a smaller set of principal components, retaining the most important features for recognition.

3. SVM for Classification:
   - A linear SVM model is trained on the reduced feature set to classify faces.
   
4. Real-Time Face Recognition:
   - OpenCV’s `CascadeClassifier` detects faces from a live video feed.
   - The detected face is projected onto the PCA space and classified using the trained SVM model.



 Future Work
- Improve accuracy by experimenting with different kernels for the SVM.
- Add a graphical user interface (GUI) for easier interaction.
- Implement face tracking to improve performance in real-time scenarios.

 Requirements
- Python 3.x
- OpenCV
- Scikit-learn
- NumPy

