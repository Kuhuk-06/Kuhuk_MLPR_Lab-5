Lab 5 – Face Detection & Clustering using Computer Vision
Aim
The aim of this project is to:

Detect faces in a group image using computer vision techniques.
Extract meaningful color-based features from detected faces.
Apply unsupervised learning (K-Means clustering) to group similar faces.
Compare a template face image against detected faces using distance metrics.
Analyze similarity using multiple mathematical distance measures.
This project demonstrates how image processing and machine learning work together for pattern recognition.

Methodology

The project follows a structured computer vision pipeline.

1. Face Detection
The group image (plaksha_Faculty.jpg) is loaded.
Converted to grayscale.
Faces are detected using OpenCV’s Haar Cascade Classifier.
Bounding boxes are drawn around detected faces.
Face Detection Output
(Insert your output image here)
![WA0011.jpg]

3. Feature Extraction
To prepare for clustering, features are extracted from each detected face:
Image converted to HSV color space
Mean Hue calculated
Mean Saturation calculated
Each face is represented as:
Feature Vector = [Mean Hue, Mean Saturation]
This transforms image data into numerical vectors suitable for machine learning.

5. K-Means Clustering
K-Means (k = 2) is applied to group faces.
Clustering is based on extracted HSV features.
Results are visualized using scatter plots.
Clustering Visualization
(Insert your clustering graph here)
![KMeans Clustering](images/kmeans_scatter_plot.png)
This visualization shows how faces are separated based on color characteristics.

6. Template Matching and Similarity Analysis
A template image (WA0010.jpg) is:
Processed similarly
Converted to HSV
Feature vector extracted
The template is then compared against detected faces using:
Euclidean Distance
Manhattan Distance
Minkowski Distance
Cosine Similarity
The closest face is identified based on minimum distance.
Distance Comparison Visualization
(Insert your distance comparison graph here)
![Distance Metrics Comparison](WA0009.jpg)
Key Findings
HSV color space reduces dimensionality while preserving meaningful information.
K-Means successfully groups visually similar faces.
Distance metrics produce slightly different similarity rankings.
Euclidean distance performed consistently for similarity comparison.
Cosine similarity works well when magnitude differences are less important than direction.

Conclusions

This project demonstrates that:
Computer vision pipelines require structured preprocessing.
Feature engineering is critical for clustering performance.
Unsupervised learning can effectively group visual data.
Mathematical distance metrics directly impact similarity-based classification.
Simple features (Hue and Saturation) can provide useful clustering results.

Limitations:

HSV features alone are not sufficient for high-accuracy facial recognition.
More advanced embeddings (e.g., deep learning-based face encoders) would significantly improve performance.

Technologies Used:

Python
OpenCV
NumPy
Matplotlib
Scikit-learn
SciPy

How to Run
Install dependencies:
pip install opencv-python numpy matplotlib scikit-learn scipy
Run:
jupyter notebook
Open:
Lab 5 final - kuhuk katiyar.ipynb
Run all cells sequentially.

Project Structure
Project Root
│── Lab 5 final - kuhuk katiyar.ipynb
│── plaksha_Faculty.jpg
│── Dr_Shashi_Tharoor.jpg
│── README.md
│── images/
      │── face_detection_output.png
      │── kmeans_scatter_plot.png
      │── distance_comparison.png
Author
Kuhuk Katiyar
