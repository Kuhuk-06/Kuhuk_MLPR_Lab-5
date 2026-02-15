Lab 5 – Face Detection & Clustering using Computer Vision
📌 Aim
The aim of this project is to:
Detect faces in a group image using computer vision techniques.
Extract meaningful color-based features from detected faces.
Apply unsupervised learning (K-Means clustering) to group similar faces.
Compare a template face image against detected faces using distance metrics.
Analyze similarity using multiple mathematical distance measures.
This project demonstrates how image processing and machine learning work together for pattern recognition.
🛠 Methodology
The project follows a structured computer vision pipeline:
1️⃣ Face Detection
The group image (plaksha_Faculty.jpg) is loaded.
Converted to grayscale.
Faces are detected using OpenCV’s Haar Cascade Classifier.
Bounding boxes are drawn around detected faces.
🔎 Face Detection Output
(Insert your output image here)
![Face Detection Output](images/face_detection_output.png)
2️⃣ Feature Extraction
To prepare for clustering, features are extracted from each detected face:
Image converted to HSV color space
Mean Hue
Mean Saturation
Each face is represented as:
Feature Vector = [Mean Hue, Mean Saturation]
This transforms image data into numerical vectors suitable for machine learning.
3️⃣ K-Means Clustering
K-Means (k = 2) is applied to group faces.
Clustering is based on extracted HSV features.
Results are visualized using scatter plots.
📊 Clustering Visualization
(Insert your clustering graph here)
![KMeans Clustering](images/kmeans_scatter_plot.png)
This visualization shows how faces are separated based on color characteristics.
4️⃣ Template Matching & Similarity Analysis
A template image (Dr_Shashi_Tharoor.jpg) is:
Processed similarly
Converted to HSV
Feature vector extracted
The template is then compared against detected faces using:
Euclidean Distance
Manhattan Distance
Minkowski Distance
Cosine Similarity
The closest face is identified based on minimum distance.
📈 Distance Comparison Visualization
(Insert your distance comparison graph here)
![Distance Metrics Comparison](images/distance_comparison.png)
📊 Key Findings
HSV color space effectively reduces dimensionality while preserving meaningful information.
K-Means successfully groups visually similar faces.
Distance metrics produce slightly different similarity rankings.
Euclidean distance performed consistently for similarity comparison.
Cosine similarity works well when magnitude differences are less important than direction.
