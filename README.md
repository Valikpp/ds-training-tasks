# 🧠 Data Science Training Tasks

Welcome to my collection of **data science and machine learning projects**.  
As a **computer science student and aspiring data scientist**, I use this repository to practice, experiment, and improve my skills on **public datasets**.  
Each project focuses on different aspects of the data science workflow — from exploratory data analysis (EDA) and feature engineering to model training, evaluation, and deployment.  

My goal is to **build a solid understanding of ML techniques** while developing clean, reproducible, and well-documented solutions.

---

## Repository Structure

Each subfolder contains a standalone project with its own dataset, notebooks, and scripts.  
Below is a brief overview of each one.

---
Data for projects : https://drive.google.com/drive/folders/1eBjre1gkmacm53og1qCbiCDNdiZFt-NX?usp=drive_link

---

### 1. `bpm`
**Description:**  
This subproject is built around a dataset containing information about various characteristics of a set of music tracks. Based on data such as rhythm, volume, instrument strength, etc., the goal is to regress the characteristic of beats per minute. 

**Task:**  
Regression of BPM

**Stage:**  
EDA → Model Training → Evaluation

**Technologies:**  
NumPy, pandas, scikit-learn, matplotlib, seaborn

**Result:**  
Best result is MSE = 26.43, (Kaggle best result = 25.xxx)
*Rem: According to data from the internet, the average bpm for music familiar to the human ear is between 80 and 180.*

---

### 2. `iris`
**Description:**  
Classic Iris dataset classification problem — predicting flower species from petal/sepal features
The aim of this subproject is to test various methods of primary analysis and visualisation using a simple example.

**Task:**  
Multiclass classification

**Stage:**  
EDA → Model Training → Model Comparison → Evaluation

**Technologies:**  
pandas, scikit-learn, matplotlib, seaborn

**Result:**  
Accuracy = 1.0

---

### 3. `titanic`
**Description:**  
Predicting passenger survival on the Titanic — Kaggle classic dataset.
The aim of this project is to use a well-known problem as an example to work on feature engineering and to test individual and combined machine learning methods.

**Task:**  
Binary classification

**Stage:**  
EDA → Feature Engineering → Model Selection → Evaluation

**Technologies:**  
pandas, NumPy, scikit-learn + GBclassifier, matplotlib

**Result:**  
Accuracy: 0.81 on validation set

---

### 4. `EmissionsCO2`
**Description:**  
Predicting CO₂ emissions from vehicle specifications.
This project is an academic project carried out as part of the lesson named "Atelier de Recherche Encadre en Data Science", with the aim of independently implementing machine learning algorithms such as the naive Bayes classifier, decision tree classifier, and knn classifier. 

**Task:**  
Project objective: using data from various sensors, determine the level of CO2 emissions into the atmosphere at a specific moment for each given timestamp.

**Stage:**  
EDA → Model Training → Feature Importance Analysis

**Technologies:**  
pandas, numpy, matplotlib


---

### 5. `CIFAR-10`
**Description:**  
A classic example of an image dataset for recognising the class of an object in it. 
Project goal: to work on augmenting the source data, implement a comprehensive approach to preparing the dataset, create a neural network architecture, and perform a training cycle. 

**Task:**  
Multiclass image classification

**Stage:**  
Preprocessing + Augmentation → CNN Model Design → Training → Evaluation → Test on real example


**Technologies:**  
PyTorch, NumPy, torchvision, matplotlib

**Result:**  
Validation accuracy = 0.85

---

### 6. `FER`
**Description:**  
Facial emotion recognition using convolutional neural networks.

**Task:**  
Multiclass image classification (emotion detection)

**Stage:**  
Data Preprocessing → CNN Model → Evaluation 

**Practical development of the project**
 During testing, it was concluded that methods based on the repeated use of CNN layers have difficulty capturing small features (which is entirely explained by their architecture). Convergence with this architecture requires an irrational number of training iterations. 
 The idea was to switch to the HRNet approach. 
 ->The goal of the project is to complete the implementation of this method and test the inference model using OpenCV for emotion recognition from video. 

**Technologies:**  
PyTorch, Torchvision, OpenCV, NumPy

**Result:**  
In 100 epochs model converges to 0.6 accuracy

---

### 7. `Morse-decoder`
**Description:**  
A large-scale comprehensive project developed during a test assignment for an internship at Kontur (Russia). The aim of the project is to use sound clips (signal recordings) to extract the Morse code contained within them. 

**Task:**  
Sequence-to-sequence audio-to-char decoding

**Stage:**  
Audio Preprocessing (Audio-to-image transformations, image preprocessing with signal) → CNN + LSTM Model → CTC Loss Training → Training and Test with different hyperparameters

**Practical development of the project**
The project is currently in the final stages of development. The latest version of the architecture and methods can be found in the `newmain.ipynb` file. At present, the problem lies in gradient vanishing and predictions being reduced to a constant symbol. 

**Technologies:**  
PyTorch, Librosa, NumPy, pandas

**Result:**  
In progress

---

### 8. `Emotions detect`
**Description:**  
A subproject aimed at developing a text processing method for assessing the emotional load of English phrases. Project goal: text data processing, tokenization, working with contextual dependencies within phrases. 

**Task:**  
Multi-label classification (Text0to-label)

**Stage:**  
EDA → Data preprocessing and Tokenization → Model Design → Evaluation

**Technologies:**  
Numpy, pandas, scikit-learn (TfidVectorizer + Logistic regression)

**Result:**  
F1-score = 0.992 (choice explained in Notebook)

---

### 9. `Stepik client dropout`
**Description:**  
The project is based on logs from the Stepik online platform and aims to analyze the reasons why online course students decide to drop out. The idea behind the project is to use a specific user's activity history to predict whether they will drop out of the course or complete it. 
The project is very interesting from a feature engineering perspective, as the raw data is completely meaningless and unsuitable for training. 

**Task:**  
Binary classification

**Stage:**  
EDA → Feature Engineering → Model Training

**Technologies:**  
Numpy, pandas, scikit-learn, matplotlib

**Result:**  
ROC-AUC = 0.73

---

### 10. `Mnist`
**Description:**  
A classic and trivial task for training with early neural networks. An old project.

**Task:**  
Multiclass classification

**Stage:**  
Data Normalization → MLP → Training → Evaluation

**Technologies:**  
PyTorch, torchvision, matplotlib

**Result:**  
Test accuracy = 96.0%

---

## Technologies Used
- **Languages:** Python  
- **Core Libraries:** pandas, NumPy, scikit-learn, PyTorch, matplotlib, seaborn  
- **ML/DL Tools:** TensorFlow, PyTorch Lightning, XGBoost, transformers (depending on project)  
- **Data Handling:** Jupyter Notebook, Google Colab  
- **Version Control:** Git, GitHub  

---

## Goals
- Improve hands-on ML skills through practical challenges  
- Explore and implement various algorithms (traditional ML and deep learning)  
- Build a portfolio demonstrating structured problem-solving in data science  

---

## Contact
If you'd like to discuss any project, or share ideas, feel free to reach out:

**GitHub:** [Valikpp](https://github.com/Valikpp)  
**Email:**
- *university email: vadim.prokhorov@etu.sorbonne-universite.fr*
- *professional email: vadim.prokhorov.prof@gmail.com*

---

## Setup & Installation

This repository contains multiple Python subprojects. To ensure all scripts run correctly, you can set up your environment using one of the two dependency files provided in the root directory.

### Option 1: Using Pip (Standard)
Best for standard Python environments or `venv`.
1. Create and activate your virtual environment.
2. Run the following command:
   ```bash
   pip install -r requirements_PIP.txt
   ```
> **Note:** This file contains a comprehensive list of Python packages required across all subprojects.

---

### Option 2: Using Conda / Mamba (Recommended)
Best if you want to reproduce the exact environment including system-level dependencies.
1. Create a new environment from the configuration file:
   ```bash
   mamba env create -f env_CONDA.yml
   ```
   *(If you don't have Mamba, you can use `conda env create -f environment.yml`)*
2. Activate the environment:
   ```bash
   mamba activate ds_ml
   ```

---

### ⚠️ Project Structure Note
Since these dependencies are bundled at the **root level**, installing them will prepare your environment for all subprojects simultaneously. If you encounter any version conflicts while running a specific script, please refer to that subproject's individual folder for more details.
