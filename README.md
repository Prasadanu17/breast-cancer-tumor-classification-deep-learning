# 🧠 Breast Cancer Tumor Classification using Deep Learning

A Deep Learning project for classifying breast tumors as **Malignant** or **Benign** using diagnostic features and a neural network model built with **Python and TensorFlow/Keras**.

## 📌 Project Overview

Breast cancer is one of the most common types of cancer worldwide. Early and accurate classification of breast tumors can assist in the analysis of diagnostic data.

In this project, a Deep Learning classification model is developed to predict whether a tumor is:

* 🔴 **Malignant (0)**
* 🟢 **Benign (1)**

The project includes data preprocessing, feature scaling, neural network training, validation, and prediction.

## 🎯 Objectives

* Analyze breast cancer diagnostic data.
* Preprocess and prepare the dataset for Deep Learning.
* Scale the input features.
* Build and train a neural network classification model.
* Evaluate training and validation performance.
* Predict whether a tumor is malignant or benign.

## 📊 Dataset

The project uses a breast cancer diagnostic dataset containing multiple numerical features describing characteristics of tumor cells.

The dataset contains **30 diagnostic features** used as model inputs.

The target variable represents the tumor classification:

| Label | Classification |
| ----: | -------------- |
|     0 | Malignant      |
|     1 | Benign         |

## 🧠 Model

A neural network model is used for binary classification.

The general workflow is:

```text
Dataset
   ↓
Data Preprocessing
   ↓
Feature / Target Separation
   ↓
Train-Test Split
   ↓
Feature Scaling
   ↓
Neural Network
   ↓
Model Training
   ↓
Validation
   ↓
Prediction
   ↓
Malignant / Benign
```

## 📈 Model Training

The model is trained using training and validation data.

Training performance is monitored using:

* Accuracy
* Validation Accuracy
* Loss
* Validation Loss

The notebook contains graphs showing the model's learning performance across epochs.

### Training vs Validation Accuracy

The accuracy graph helps visualize how the model's classification performance changes during training.

### Training vs Validation Loss

The loss graph helps analyze the model's error during training and validation.

## 🔮 Prediction

After training, new diagnostic feature values can be provided to the model.

The input data is first transformed using the same scaler used during training:

```python
scaled_input = scaler.transform(input_data)
```

The trained model then generates prediction probabilities:

```python
prediction = model.predict(scaled_input)
```

The predicted class is obtained using:

```python
predicted_class = np.argmax(prediction)
```

The output is interpreted as:

```text
0 → Malignant
1 → Benign
```

## 🛠️ Technologies Used

* 🐍 Python
* 🧠 TensorFlow
* Keras
* NumPy
* Pandas
* Scikit-learn
* Matplotlib
* Jupyter Notebook

## 📂 Project Structure

```text
breast-cancer-tumor-classification-deep-learning/
│
├── 📓 breast_cancer.ipynb
├── 📊 data.csv
├── 📄 README.md
└── 📁 .git/
```

### `breast_cancer.ipynb`

Contains the complete implementation including:

* Data loading
* Data preprocessing
* Exploratory analysis
* Feature scaling
* Model creation
* Model training
* Validation
* Performance visualization
* Prediction

### `data.csv`

Contains the dataset used for training and evaluating the model.

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone https://github.com/Prasadanu17/breast-cancer-tumor-classification-deep-learning.git
```

### 2. Navigate to the project

```bash
cd breast-cancer-tumor-classification-deep-learning
```

### 3. Install the required libraries

```bash
pip install numpy pandas matplotlib scikit-learn tensorflow jupyter
```

### 4. Start Jupyter Notebook

```bash
jupyter notebook
```

### 5. Open the notebook

Open:

```text
breast_cancer.ipynb
```

Run the cells sequentially to train the model and generate predictions.

## 📌 Key Learning Outcomes

Through this project, I gained practical experience in:

* Data preprocessing
* Feature scaling
* Train-test splitting
* Neural network development
* Deep Learning model training
* Model validation
* Classification
* Prediction using trained models
* Data visualization
* TensorFlow/Keras

## 🔮 Future Improvements

Possible improvements for this project include:

* Adding a confusion matrix
* Adding precision, recall, and F1-score
* Comparing different machine learning models
* Hyperparameter tuning
* Improving model architecture
* Adding a Streamlit web interface
* Deploying the model as a web application
* Adding an interactive prediction form

## ⚠️ Disclaimer

This project is developed for **educational and research purposes only**. It is not intended to replace professional medical diagnosis, clinical evaluation, or medical advice.

## 👩‍💻 Author

**Anu Kumari Shah**

MCA Student | AI/ML & Web Development Enthusiast

Interested in:

* Artificial Intelligence
* Machine Learning
* Deep Learning
* Data Science
* Natural Language Processing
* Web Development

---

⭐ If you find this project useful, consider giving the repository a star!
