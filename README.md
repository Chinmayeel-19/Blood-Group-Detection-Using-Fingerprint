# Blood Group Detection Using Fingerprint

A deep learning-based academic project that explores fingerprint image classification using a Convolutional Neural Network (CNN), TensorFlow, OpenCV, and Flask.

The project provides a web interface where users can upload a fingerprint image and receive a model-generated blood group prediction.

## Project Overview

This project uses a trained CNN model to classify fingerprint images into eight blood group categories. A Flask application connects the trained model to a simple web interface for image upload and prediction.

**Key highlights**
- CNN-based fingerprint image classification
- Eight output classes: A+, A-, B+, B-, AB+, AB-, O+, O-
- Image preprocessing using TensorFlow/Keras
- Fingerprint image resizing to 64 × 64 pixels
- Flask-based web application
- Prediction output with the model's returned confidence score
- Pre-trained model included in the repository

## Tech Stack

| Category | Technologies |
|---|---|
| Programming Language | Python |
| Deep Learning | TensorFlow, Keras |
| Image Processing | OpenCV, Pillow |
| Machine Learning | Scikit-learn |
| Web Framework | Flask |
| Data Handling | NumPy, Pandas |
| Development Tools | Jupyter Notebook, VS Code |

## Project Structure

```text
Blood-Group-Detection-Using-Fingerprint/
│
├── dataset/
│   └── dataset_blood_group/
│       ├── A+/
│       ├── A-/
│       ├── B+/
│       ├── B-/
│       ├── AB+/
│       ├── AB-/
│       ├── O+/
│       └── O-/
│
├── model/
│   └── model.h5
│
├── notebook/
│   └── bloodgrpclassificationfromfingerprint.ipynb
│
├── static/
│   ├── spinner.gif
│   └── spinner1.gif
│
├── templates/
│   └── index.html
│
├── uploads/
│
├── app.py
├── requirements.txt
├── Procfile
├── .gitignore
└── README.md
```

## Dataset

- Contains approximately 6,000 fingerprint images.
- Images are organized into eight blood group folders.
- The dataset images are stored in BMP format.
- The dataset is used for model training and classification.

## How It Works

1. **Image Upload:** The user uploads a fingerprint image through the Flask web interface.
2. **Image Validation:** The application checks the uploaded file format.
3. **Preprocessing:** The image is resized to 64 × 64 pixels and converted into a numerical array.
4. **Model Prediction:** The pre-trained CNN model processes the image.
5. **Classification:** The application selects the predicted class from the eight blood group labels.
6. **Result Display:** The prediction label and model confidence score are returned.

## Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/Chinmayeel-19/Blood-Group-Detection-Using-Fingerprint.git
```

### 2. Navigate to the project directory

```bash
cd Blood-Group-Detection-Using-Fingerprint
```

### 3. Create a virtual environment

```bash
python -m venv .venv
```

### 4. Activate the environment

**Windows:**

```bash
.venv\Scripts\activate
```

### 5. Install dependencies

```bash
pip install -r requirements.txt
```

### 6. Run the Flask application

```bash
python app.py
```

### 7. Open the application

Visit the following address in your browser:

```text
http://127.0.0.1:5000/
```

Upload a supported fingerprint image to test the application.

## Supported Image Formats

- JPG
- JPEG
- PNG
- BMP

## Model Information

- Model type: Convolutional Neural Network (CNN)
- Framework: TensorFlow / Keras
- Input image dimensions: 64 × 64 pixels
- Output classes: 8 blood group categories
- Saved model: `model/model.h5`

## Future Enhancements

- Improve model performance through further experimentation and validation.
- Add model evaluation metrics and visualizations.
- Improve error handling and image validation.
- Enhance the web interface and user experience.
- Explore explainable AI techniques for model interpretation.

## Important Disclaimer

This project is developed for academic and educational purposes only. It is an experimental fingerprint image classification project and is not a clinically validated method for determining blood group.

Blood group determination for medical care and transfusion decisions requires validated laboratory testing. Never use this application's predictions for medical decisions, blood donation eligibility, or transfusions.

## Author

**Chinmayeel-19**

GitHub: [github.com/Chinmayeel-19](https://github.com/Chinmayeel-19)

---

If you find this project useful, feel free to explore the repository and its implementation.
