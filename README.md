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
   git clone https://github.com/Devansh-Gupta-Official/Body-Language-Decoder.git
   ```
2. **Install Dependencies:**
   ```
   pip install -r requirements.txt
   ```
   
## **Usage**
1. **Run the main script:**
   ```
   python code.py
   ```
2. **Prepare Webcam:**
   - Ensure your webcam is connected and properly positioned.
   - Have sufficient lighting for accurate landmark detection.
3. **Gesture Recognition:**
   - Perform gestures in front of the camera to see real-time recognition results.
   - The recognized body language class and its probability will be displayed on the screen.
  

## **File Structure:**
```
├── coden.py     # Main script for data collection and recognition
├── coords.csv                       # CSV file containing collected coordinates
├── body_language.pkl                # Pickled model file
└── README.md                        # Project readme file
```

## **Requirements:**
- Python 3.x
- OpenCV: Python library for computer vision tasks.
- Mediapipe: Google's framework for building multimodal applied machine learning pipelines.
- Pandas: Data manipulation and analysis library.
- Scikit-learn: Machine learning library for Python.

## **Results:**
![image](https://github.com/Devansh-Gupta-Official/Body-Language-Decoder/assets/100591612/4fc1e7e5-bbcf-4447-9548-9f37662f878e)
![image](https://github.com/Devansh-Gupta-Official/Body-Language-Decoder/assets/100591612/1b8dfb6a-d502-4322-9fae-9dadee9ffbc7)
![image](https://github.com/Devansh-Gupta-Official/Body-Language-Decoder/assets/100591612/c44c7b27-7f84-4860-95a1-5c08282d1f96)




