 Speech Emotion Recognition using Spectrogram-Based CNN Models

 Overview

This project implements a **Speech Emotion Recognition (SER)** system using deep learning and classical machine learning techniques. The objective is to classify human emotions from speech signals using time–frequency audio representations such as **Mel Spectrograms** and **MFCC features**.

The system evaluates multiple models including **Convolutional Neural Networks (CNN)** and traditional machine learning algorithms such as **Random Forest** and **Support Vector Machines (SVM)**.

The experiments are conducted on the **RAVDESS Emotional Speech Dataset**, and additional analysis is performed to study emotion-specific spectrogram patterns.

---

 Key Features

* Speech emotion classification using deep learning
* Feature extraction using **Mel Spectrograms** and **MFCC**
* Comparison of multiple machine learning models
* Emotion confusion analysis using confusion matrices
* Emotion-specific spectrogram pattern analysis
* Visualization of acoustic patterns across emotions

---

 Dataset

This project uses the **RAVDESS Emotional Speech Dataset**.

Download the dataset from:
https://www.kaggle.com/datasets/uwrfkaggler/ravdess-emotional-speech-audio

After downloading, place the dataset in the project directory:


Speech-Emotion-Recognition/
│
├── RAVDESS Emotional speech audio/


The dataset is **not included in this repository** due to its size.

---

 Project Structure

```
Speech-Emotion-Recognition
│
├── notebook
│   └── speech_emotion_recognition.ipynb
│
├── images
│   ├── spectrogram_examples.png
│   ├── confusion_matrix.png
│   └── model_comparison.png
│
├── requirements.txt
├── README.md
└── .gitignore


---

 Feature Extraction

Two types of audio features are used:

 1. Mel Spectrogram

A time–frequency representation of the audio signal used for training the CNN model.

 2. MFCC (Mel Frequency Cepstral Coefficients)

Compact acoustic features widely used in speech processing tasks.

---

 Implemented Models

The following models were implemented and compared:

| Model         | Feature Type    | Accuracy |
| ------------- | --------------- | -------- |
| CNN           | Mel Spectrogram | 92.9%    |
| Random Forest | MFCC            | 92.7%    |
| SVM           | MFCC            | 79.8%    |

The CNN model achieved the best performance by learning spatial patterns from spectrogram representations of speech signals.

---

 Emotion Confusion Analysis

A confusion matrix was generated to analyze classification errors.

Common confusion patterns observed:

* Fear vs Surprise
* Calm vs Neutral

These emotions share similar acoustic characteristics, making them more difficult to distinguish.

---

 Emotion-Specific Spectrogram Analysis

Spectrogram visualization reveals distinctive acoustic patterns across emotional states.

Key observations:

* **Angry speech** contains strong high-frequency energy components.
* **Sad speech** shows lower frequency dominance and reduced spectral variation.
* **Happy speech** exhibits dynamic frequency changes.
* **Calm and neutral speech** display relatively stable spectral patterns.

These findings confirm that emotional speech signals contain unique frequency-energy distributions that can be captured by deep learning models.

---

 Installation

Clone the repository:

```

```

Navigate to the project folder:

```
cd Speech-Emotion-Recognition
```

Install dependencies:

```
pip install -r requirements.txt
```

---

 Running the Project

Open the Jupyter notebook:

```
jupyter notebook
```

Then run:

```
speech_emotion_recognition.ipynb
```

The notebook performs:

* Data preprocessing
* Feature extraction
* Model training
* Evaluation and visualization

---

 Technologies Used

* Python
* NumPy
* Pandas
* Librosa
* Scikit-learn
* TensorFlow / Keras
* Matplotlib
* Seaborn
* Jupyter Notebook

---

 Results Visualization

The project includes visualizations such as:

* Mel Spectrograms
* Emotion-wise average spectrograms
* Confusion matrix
* Model comparison charts

These visualizations help interpret how different emotions manifest in speech signals.

---

 Future Improvements

Possible improvements include:

* Hyperparameter optimization
* Data augmentation for audio signals
* Advanced deep learning architectures
* Transformer-based speech models
* Explainable AI techniques such as Grad-CAM for audio models

---

 Author

Saptarshi Debnath


---


