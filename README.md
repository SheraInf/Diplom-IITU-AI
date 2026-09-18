# AI-Based Industrial Defect Detection System

## Diploma Project

**Group:** IT3-2401AI

**Students:**

* **Sherkhan Yerkebay**
* **Abdikul Dastan**
* **Ablez Damir**

---

## Project Description

This project is a Deep Learning-based intelligent system for automatic detection and classification of defects on industrial product surfaces.

The main purpose of the system is to automate visual quality inspection using computer vision and deep neural networks. The system analyzes an uploaded image, detects possible defects, determines their type, and provides the confidence of the prediction.

The project combines **Deep Learning, Computer Vision, Backend Development, Database Technologies, and Web Development** into a single application.

### Main Workflow

```text
Input Image
     │
     ▼
Image Preprocessing
     │
     ▼
Deep Learning Model
     │
     ▼
Defect Detection
     │
     ▼
Defect Classification
     │
     ▼
Confidence Score
     │
     ▼
Web Interface
```

---

## Objectives

The main objectives of the project are:

1. Analyze existing approaches for automated industrial defect detection.
2. Prepare and preprocess an image dataset.
3. Develop and train Deep Learning models for defect detection and classification.
4. Compare the performance of different neural network architectures.
5. Implement an inference pipeline for analyzing new images.
6. Develop a backend API for communication with the AI model.
7. Create a web interface for uploading images and displaying detection results.
8. Store and visualize inspection results.
9. Evaluate the developed system using standard machine learning metrics.

---

## Key Features

* Upload industrial product images.
* Automatic defect detection.
* Defect classification.
* Confidence score for predictions.
* Visualization of detected defect areas.
* Image preprocessing and augmentation.
* Deep Learning model inference.
* REST API for AI model interaction.
* Inspection history.
* Statistical analysis of model results.
* Web-based user interface.

---

## Dataset

The project is designed to work with publicly available industrial defect datasets.

Potential datasets include:

* **NEU Surface Defect Database**
* **MVTec AD**
* **MVTec AD 2**

These datasets contain images of industrial surfaces with different types of defects and are widely used for research in computer vision and anomaly detection.

### Example Defect Classes

Depending on the selected dataset, the system may detect:

* Scratches
* Cracks
* Surface contamination
* Inclusions
* Pitted surfaces
* Patches
* Rolled-in scale
* Other abnormal surface patterns

The final dataset and class configuration will be specified according to the selected experimental setup.

---

## Deep Learning

The main part of the project is the Deep Learning model responsible for analyzing images.

The experimental pipeline may include several architectures for comparison:

```text
Dataset
   │
   ├── Preprocessing
   │
   ├── Data Augmentation
   │
   ▼
Training
   │
   ├── CNN / ResNet
   ├── EfficientNet
   ├── YOLO
   └── Vision Transformer
   │
   ▼
Model Evaluation
   │
   ▼
Best Model
```

The final model will be selected based on experimental results rather than only theoretical characteristics.

### Evaluation Metrics

The following metrics can be used:

* Accuracy
* Precision
* Recall
* F1-score
* ROC-AUC
* mAP
* Inference time

For object detection and localization, additional metrics may be used depending on the selected architecture.

---

## System Architecture

The planned architecture consists of three major layers.

```text
┌───────────────────────────────┐
│          Frontend             │
│                               │
│ Image Upload                  │
│ Detection Results             │
│ Statistics / Dashboard        │
└───────────────┬───────────────┘
                │
                │ HTTP / REST API
                ▼
┌───────────────────────────────┐
│           Backend             │
│                               │
│ FastAPI                       │
│ Authentication                │
│ Image Processing              │
│ Database Communication        │
└───────────────┬───────────────┘
                │
                ▼
┌───────────────────────────────┐
│       Deep Learning           │
│                               │
│ Trained Model                 │
│ Image Preprocessing           │
│ Defect Detection              │
│ Classification                │
└───────────────┬───────────────┘
                │
                ▼
┌───────────────────────────────┐
│          Database             │
│                               │
│ Users                         │
│ Images                        │
│ Predictions                   │
│ Inspection History            │
└───────────────────────────────┘
```

---

## Project Structure

The project is organized into several main components:

```text
Diplom-IITU-AI/
│
├── dataset/
│   ├── train/
│   ├── validation/
│   └── test/
│
├── models/
│   └── trained_models/
│
├── backend/
│   ├── api/
│   ├── services/
│   ├── database/
│   └── main.py
│
├── frontend/
│   ├── src/
│   ├── public/
│   └── package.json
│
├── notebooks/
│   ├── data_preparation.ipynb
│   ├── model_training.ipynb
│   └── model_evaluation.ipynb
│
├── tests/
│
├── requirements.txt
│
└── README.md
```

The exact structure may change during development.

---

## Technologies

### Artificial Intelligence

* Python
* PyTorch / TensorFlow
* OpenCV
* NumPy
* Pandas
* Scikit-learn
* YOLO
* CNN architectures

### Backend

* Python
* FastAPI
* REST API
* PostgreSQL / SQLite

### Frontend

* HTML
* CSS
* JavaScript
* React (planned)

### Development Tools

* Git
* GitHub
* PyCharm / VS Code
* Jupyter Notebook
* Google Colab

---

## Development Team

### Sherkhan Yerkebay

**Area of responsibility:**

* Deep Learning
* Dataset preparation
* Model training
* Model evaluation
* Computer Vision

### Abdikul Dastan

**Area of responsibility:**

* Backend development
* REST API
* Database
* AI model integration
* Server-side processing

### Ablez Damir

**Area of responsibility:**

* Frontend development
* User interface
* Visualization
* Dashboard
* Integration with backend API

---

## Development Stages

### Phase 1 — Research

* Analyze existing industrial defect detection systems.
* Analyze available datasets.
* Study Deep Learning architectures.
* Define system requirements.

### Phase 2 — Dataset Preparation

* Download the selected dataset.
* Clean and organize the data.
* Resize images.
* Normalize data.
* Apply data augmentation.
* Divide data into training, validation, and test sets.

### Phase 3 — Model Development

* Implement baseline model.
* Train several Deep Learning architectures.
* Tune hyperparameters.
* Compare model performance.
* Select the final model.

### Phase 4 — Backend

* Develop REST API.
* Implement image upload.
* Connect the trained model.
* Process predictions.
* Store results in the database.

### Phase 5 — Frontend

* Create image upload interface.
* Display detection results.
* Visualize detected defects.
* Implement inspection history.
* Add statistics and charts.

### Phase 6 — Testing

* Test model accuracy.
* Test API functionality.
* Test frontend/backend integration.
* Measure inference time.
* Test different image inputs.

### Phase 7 — Final Evaluation

The final system will be evaluated based on:

* Detection/classification quality.
* Model performance.
* Processing speed.
* System reliability.
* Usability.
* Accuracy of integration between components.

---

## Expected Result

The final result of the project will be a web-based intelligent quality inspection system.

A user will be able to upload an image of an industrial product and receive an automated analysis:

```text
Image
  ↓
AI Analysis
  ↓
Defect Found
  ↓
┌──────────────────────────┐
│ Defect: Scratch          │
│ Confidence: 96.4%        │
│ Location: detected area  │
└──────────────────────────┘
```

The system will also provide a visual representation of the detected defect and store the inspection result for further analysis.

---

## Research Component

An important part of the diploma project is the experimental comparison of Deep Learning approaches.

The research will investigate how different architectures perform on the selected industrial defect dataset.

The comparison may include:

```text
Model A ──┐
Model B ──┤
Model C ──┼──► Evaluation ──► Comparison
Model D ──┤
Model E ──┘
```

The models will be compared using common evaluation metrics and computational characteristics.

This allows the project to include not only software development but also an experimental research component.

---

## Future Improvements

Possible future improvements include:

* Real-time camera-based inspection.
* Video stream defect detection.
* Model optimization for edge devices.
* Mobile application.
* Additional industrial datasets.
* Anomaly detection for previously unknown defect types.
* Explainable AI techniques.
* Model quantization and acceleration.
* Integration with industrial monitoring systems.

---

## Academic Information

**University:** International Information Technology University (IITU)

**Group:** IT3-2401AI

**Project Type:** Diploma Project

**Field:** Artificial Intelligence / Deep Learning / Computer Vision

**Academic Year:** 2026

---

## License

This project is developed for academic and educational purposes as part of the diploma project of the IT3-2401AI group.
