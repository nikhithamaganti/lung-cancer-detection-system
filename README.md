
Project: Lung Cancer Detection System using Machine Learning and CNN

- Nikhitha Maganti


Overview
--------
This project implements a machine learning and deep learning pipeline to detect lung cancer from CT scan images. The system includes image preprocessing, feature extraction using PCA, and classification using multiple algorithms such as SVM, KNN, K-Means, and CNN. The project also provides a GUI-based interface for user interaction and real-time prediction.

Directory Structure
------------------
lungs/
├── Title1_SVM_KMeans/
│   ├── SVM_KMEANS.py          - GUI application for SVM vs K-Means
│   ├── test.py                - Feature generation script
│   ├── features/              - Generated feature files (X.txt.npy, Y.txt.npy)
│   ├── testSamples/           - Sample images for prediction
│
├── Title2_SVM_KNN/
│   ├── SVM_KNN.py             - GUI application for SVM vs KNN
│   ├── features/              - Feature files
│   ├── testSamples/           - Sample images
│
├── Title3_SVM_CNN/
│   ├── SVM_CNN.py             - GUI application for SVM vs CNN
│   ├── features/              - Feature files
│   ├── testSamples/           - Sample images
│
├── Title4_SVM_CNN_Accuracy/
│   ├── SVM_CNN_Accuracy.py    - Accuracy comparison of SVM and CNN
│   ├── features/              - Feature files
│   ├── testSamples/           - Sample images
│
├── Dataset/
│   ├── normal/                - Normal CT scan images
│   ├── abnormal/              - Abnormal CT scan images
│
├── screens.docx               - Screenshots of outputs
├── README.txt                - Project instructions


Prerequisites
-------------
- Windows 10 or later
- Python 3.8 or later
- VS Code / Command Prompt
- Internet connection (for installing libraries)

Setup Instructions
------------------
1. Install Python:
   - Download Python from https://www.python.org/downloads/
   - Ensure "Add Python to PATH" is selected

2. Install Required Libraries:
   Open terminal and run:

   pip install numpy pandas matplotlib opencv-python scikit-learn tensorflow

3. Verify Dataset:
   - Ensure Dataset folder contains:
     - normal/
     - abnormal/

Running the Project
-------------------
1. Navigate to Project Folder:
   cd path\to\lungs

2. Run Title 1 (SVM vs K-Means):
   cd Title1_SVM_KMeans
   python SVM_KMEANS.py

3. Run Title 2 (SVM vs KNN):
   cd ..
   cd Title2_SVM_KNN
   python SVM_KNN.py

4. Run Title 3 (SVM vs CNN):
   cd ..
   cd Title3_SVM_CNN
   python SVM_CNN.py

5. Run Title 4 (Accuracy Comparison):
   cd ..
   cd Title4_SVM_CNN_Accuracy
   python SVM_CNN_Accuracy.py

6. GUI Instructions:
   - Click "Upload Dataset"
   - Click "Read & Split Dataset"
   - Execute algorithms
   - View graph and prediction results

Expected Outputs
---------------
- Accuracy / Error Rate displayed in GUI
- Graph comparing model performance
- Prediction result (Normal / Abnormal) on CT scan images
- CNN training logs (epochs and accuracy)

Troubleshooting
---------------
- If features not found:
  Run test.py in Title1 to generate feature files

- If image not loading:
  Ensure testSamples folder contains valid images

- If TensorFlow errors occur:
  Update import statements to use tensorflow.keras

- If GUI freezes:
  Close OpenCV image window properly

Dataset
-------
Custom dataset of lung CT scan images categorized into:
- Normal
- Abnormal