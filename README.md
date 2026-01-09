# YT Sanitizer

**YouTube Spam Detection and Filtering System**

YT Sanitizer is a machine learning project designed to automatically detect and filter spam comments on YouTube videos. The project demonstrates data preprocessing, feature extraction, model training, evaluation, and visualization, providing a clear workflow for text-based spam detection.

---

## Table of Contents
1. [Project Overview](#project-overview)
2. [Folder Structure](#folder-structure)
3. [Features](#features)
4. [Installation](#installation)
5. [Usage](#usage)
6. [Dataset](#dataset)
7. [Contributing](#contributing)
8. [License](#license)

---

## Project Overview

YT Sanitizer leverages classical NLP techniques and machine learning algorithms to classify YouTube comments as **spam** or **ham (non-spam)**.  
The main goals of this project are:

- Analyze YouTube comments for spam patterns  
- Preprocess text data (tokenization, stopwords removal, TF-IDF)  
- Train and compare machine learning models (e.g., Naive Bayes, Logistic Regression, SVM)  
- Evaluate models using accuracy, confusion matrix, and other metrics  
- Visualize results with plots and charts  

---

## Folder Structure

YT-Sanitizer/  
│  
├── data/  
│ ├── raw/ # Original dataset CSV  
│ └── processed/ # Cleaned/preprocessed data  
│
├── notebooks/ # Jupyter notebooks  
│ ├── 01_data_exploration.ipynb  
│ ├── 02_preprocessing.ipynb  
│ ├── 03_model_training.ipynb  
│ └── 04_evaluation.ipynb  
│  
├── src/ # Reusable scripts  
│ ├── preprocessing.py  
│ ├── features.py  
│ ├── train.py  
│ └── evaluate.py  
│  
├── models/ # Trained models  
│ └── yt_sanitizer_model.pkl  
│  
├── requirements.txt # Project dependencies  
├── README.md # This file  
└── .gitignore # Ignore venv, cache, checkpoints  

`yaml

---

## Features

- Detect spam comments automatically  
- Preprocess text data with NLP techniques  
- Multiple ML models for comparison  
- Model evaluation and visualization  
- Clean and modular project structure suitable for collaboration

---

## Installation

1. **Clone the repository**
```bash
git clone https://github.com/your-username/YT-Sanitizer.git  
cd YT-Sanitizer  
```

2. **Create a virtual environment**
```bash
python -m venv .venv
```

3. **Activate the environment**
```bash
# Windows
.venv\Scripts\activate

# macOS/Linux
source .venv/bin/activate
```

4. **Install required packages**
```bash
pip install -r requirements.txt
```

5. **Set up Jupyter kernel**
```bash
python -m ipykernel install --user --name yt_sanitizer --display-name "Python (YT Sanitizer)"
```

## Dataset
The project uses a **YouTube Spam Comments dataset** with labeled comments (`spam` or `ham`).  
- `comment_text` → The text of the comment  
- `label` → 1 for spam, 0 for non-spam
Souce: https://archive.ics.uci.edu/dataset/380/youtube+spam+collection
