# Body Language Recognition using Mediapipe and Machine Learning

## **Overview**
This project focuses on real-time body language recognition using Mediapipe, OpenCV, and Machine Learning. It leverages pose estimation and face landmarks to classify body language gestures captured via webcam. The system identifies and predicts various body language postures, aiding in applications related to human-computer interaction and non-verbal communication analysis.

## **How it Works**
The project is divided into two primary components:

### Data Collection
- **Webcam Feed Capture:**
  Accesses the webcam feed using OpenCV.
- **Landmark Extraction:**
  Utilizes Mediapipe to extract pose and face landmarks in real time.
- **Data Recording:**
  Records the 3D coordinates and visibility for each landmark.
- **Data Storage:**
  Saves the collected data into a CSV file for subsequent model training.

### Model Training and Real-time Recognition
- **Data Preparation:**
  - Loads the collected CSV file containing landmark data.
  - Splits the dataset into training and testing sets.
- **Machine Learning Models:**
  Employs various classifiers:
  - Logistic Regression
  - Ridge Classifier
  - Random Forest Classifier
  - Gradient Boosting Classifier
- **Model Training and Evaluation:**
  - Trains the models on the training set.'
  - Evaluates model accuracy on the test set.
- **Model Persistence:**
  Saves the best-performing model using Pickle for real-time recognition.

## **Installation**
1. **Clone the repository:**
   ```
   git clone https://github.com/Devanshh-Gupta-Official/Body-Language-Decoder.git
   ```
2. **Install Dependencies:**
   ```
   pip install -r requirements.txt
   ```


