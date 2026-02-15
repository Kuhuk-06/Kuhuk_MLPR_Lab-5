# Kuhuk_MLPR_Lab-5
Lab 5 – Face Detection and Clustering using Computer Vision
Overview
This project implements face detection, feature extraction, clustering, and similarity comparison using Python and computer vision techniques.
The notebook performs the following tasks:
Detects faces in a group image using Haar Cascade Classifier
Extracts color-based features (Hue and Saturation) from detected faces
Applies K-Means clustering to group similar faces
Visualizes clusters using scatter plots
Compares detected faces with a template image using distance-based similarity
The project demonstrates the practical application of image processing, unsupervised learning, and distance-based classification concepts.
Technologies Used
Python 3
OpenCV (cv2)
NumPy
Matplotlib
Scikit-learn (KMeans)
SciPy (distance metrics)
Project Structure
Lab 5 final - kuhuk katiyar.ipynb
plaksha_Faculty.jpg
Dr_Shashi_Tharoor.jpg
README.md
How It Works
1. Face Detection
The group image (plaksha_Faculty.jpg) is loaded.
It is converted to grayscale.
Haar Cascade classifier is used to detect faces.
2. Feature Extraction
The image is converted to HSV color space.
For each detected face:
Mean Hue
Mean Saturation
are computed as feature vectors.
3. Clustering
K-Means clustering is applied on the extracted features.
Faces are grouped into two clusters.
Results are visualized using scatter plots.
4. Template Matching
A template image (Dr_Shashi_Tharoor.jpg) is processed.
Its Hue and Saturation features are extracted.
Distance metrics are used to compare the template with clustered faces.
The closest match is identified.
Key Concepts Used
Haar Cascade Face Detection
HSV Color Space
Feature Engineering
K-Means Clustering
Distance Metrics:
Euclidean Distance
Manhattan Distance
Minkowski Distance
Cosine Similarity
How to Run
Clone the repository:
git clone <your-github-repo-link>
Install dependencies:
pip install opencv-python numpy matplotlib scikit-learn scipy
Open the notebook:
jupyter notebook
Run all cells sequentially.
Make sure the required images are in the same directory as the notebook.
Report Section
The notebook includes conceptual questions at the end.
The report answers:
Common distance metrics used in classification algorithms
Their role in measuring similarity between feature vectors
Learning Outcomes
By completing this project, you demonstrate understanding of:
Real-world face detection implementation
Extracting meaningful image features
Applying unsupervised learning (K-Means)
Using distance-based similarity comparison
Visualizing clustering results
👩‍💻 Author
Kuhuk Katiyar
