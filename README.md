# Doorlock System with Face Recognition

## Project Description
This project is a sophisticated doorlock system that integrates real-time face recognition using a Convolutional Neural Network (CNN) model. The system captures face images, preprocesses the data, trains a CNN model, and performs real-time face recognition to grant access. This project enhances security and provides a modern, hands-free access control solution.

## Features
- **Real-time Face Recognition**: Uses a trained CNN model for identifying faces.
- **Image Data Collection**: Captures face images using a webcam or IP camera.
- **Data Preprocessing**: Processes and prepares the image data for training.
- **Model Training**: Trains a CNN model on collected face data.
- **Secure Access Control**: Grants or denies access based on face recognition results.

## Installation
Follow these steps to set up the project on your local machine:

1. **Clone the Repository**:
   
   ```sh
   git clone https://github.com/your-username/doorlock-system.git
   cd doorlock-system
   
2. **Create Virtual Environment**:
   python3 -m venv venv
   source venv/bin/activate
   
3. **Install Dependencies**:
   pip install -r requirements.txt

4. **Download and Place Haarcascade File**:
   Download the haarcascade_frontalface_default.xml from OpenCV GitHub and place it in 
   the model directory.

## Usage
1. **Data Collection**:
   Run the data collection script to capture face images:

   python model/data_collection.py

   Follow the on-screen instructions to capture and save images.

2. **Data Preprocessing**:

   Run the data preprocessing script:
   
   python model/data_preprocessing.py
   
3. **Model Training**:

  Train the CNN model on the preprocessed data:

  python model/train_model.py

4. **Real-time Face Recognition**:

   Run the face recognition script to start real-time face recognition:

   python model/face_recognition.py

## Directory Structure:

doorlock-system/
├── backend/
├── data/
│   ├── images/
│   └── clean_data/
├── doorlock/
├── frontend/
├── model/
│   ├── data_collection.py
│   ├── data_preprocessing.py
│   ├── train_model.py
│   ├── face_recognition.py
│   └── final_model.h5
├── scripts/
├── 3Dmodels/
├── requirements.txt
└── README.md

## Contribution Guidelines
Contributions are welcome! To contribute to this project, please follow these steps:

1. Fork the repository.
2. Create a new branch (git checkout -b feature-branch).
3. Make your changes and commit them (git commit -am 'Add new feature').
4. Push to the branch (git push origin feature-branch).
5. Create a new Pull Request.

**License**
This project is licensed under the MIT License. See the LICENSE file for more details.

**Acknowledgments**

1. Thanks to the OpenCV community for providing the Haar Cascade classifier.
2. Special thanks to all contributors and collaborators.

This `README.md` file provides a comprehensive overview of your project, including installation and usage instructions, which will help other users and contributors understand and work with your doorlock system project.
