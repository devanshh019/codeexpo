# 🚨 AI Emergency Call Triage & Dispatch Optimizer

An **AI-powered multimodal emergency analysis system** that analyzes emergency calls using **text, speech emotion, and background sounds** to determine the **urgency level** of a situation and help dispatch teams prioritize responses.

This project was presented at **Amiphoria 2026 – CodeCraft Expo at Amity University Jharkhand**.

---

# 📌 Problem Statement

Emergency call centers receive thousands of calls daily.  
Human operators must quickly determine **how critical a situation is**, often under pressure and with incomplete information.

Important signals in a call include:
- Caller **speech emotion**
- **Background sounds** (gunshots, crashes, screams, fire alarms)
- **Verbal description** of the situation

Our system analyzes all these signals using **Multimodal AI** to generate an **urgency score** that can help emergency services prioritize dispatch.

---

# 🧠 System Overview

The system processes **three different modalities**:

1. **Speech Emotion Detection**
2. **Background Sound Classification**
3. **Emergency Text Classification**

The outputs from these models are combined using a **Fusion Model** that predicts the final **urgency level**.

---

# 🏗 Model Architecture

## 1️⃣ Emotion Detection Model

Detects emotional state of the caller.

**Input**
Voice audio

**Feature Extraction**
Mel Spectrogram (128 × 200)

**Model Architecture**
CNN + LSTM Hybrid Network

**Output**
Emotion feature vector

Example emotions:
- Panic
- Fear
- Anger
- Distress
- Neutral

---

## 2️⃣ Background Sound Detection Model

Detects environmental sounds that may indicate danger.

**Input**
Background audio

**Feature Extraction**
MFCC (40 dimensional)

**Model**
CNN classifier

**Example detected sounds**
- Gunshots
- Car crashes
- Screams
- Fire alarms
- Traffic chaos

Dataset used:
UrbanSound8K

---

## 3️⃣ Emergency Text Classification Model

Classifies the content of the emergency call.

**Input**
Transcribed text

**Vectorization**
TF-IDF

**Model**
Machine Learning classifier

**Example classes**
- Medical Emergency
- Fire
- Crime
- Accident
- Natural Disaster
- Violence
- Rescue Request

---

# 🔗 Fusion Model (Multimodal Intelligence)

The fusion model is the **core component of the system**.

Each modality produces **feature vectors**:

Emotion Model → Emotion feature vector  
Background Model → Sound feature vector  
Text Model → Text feature vector  

These features are **combined into a single dataset**.

## Fusion Pipeline

Step 1  
Extract features from all three models

Step 2  
Concatenate feature vectors

Step 3  
Feed combined vector into fusion neural network

## Fusion Network

Input Layer  
Combined multimodal feature vector

Hidden Layers  
Dense neural network layers that learn interactions between modalities

Output Layer  
Predicted **Urgency Score / Priority Level**

Example:

Calm text but panic voice + crash sounds  
→ High urgency prediction

---

# ⚙️ Tech Stack

## Programming
Python

## Machine Learning
TensorFlow  
Keras  
Scikit-learn  

## Audio Processing
Librosa  
Mel Spectrogram  
MFCC

## Natural Language Processing
TF-IDF Vectorization  
Text Classification Models

## Deployment
Streamlit

## Datasets
UrbanSound8K  
RAVDESS Emotional Speech Dataset  
Custom Synthetic Emergency Dataset

---

# 🖥 Demo

Streamlit dashboard allows users to:

- Input emergency text
- Upload audio files
- Analyze emotion and background sounds
- Generate urgency prediction

Live App  
https://emergencycalldeployed-gvybmfheowhghrazvugimh.streamlit.app

---


---

# 👥 Team

**Devansh Kumar**  
Machine Learning & Multimodal Fusion

**Arushi Kumari**  
Machine Learning & Natural Language Processing Model

**Warisha**  
Frontend & Website Interface

---

# 🚀 Future Improvements

- Real-time emergency call processing
- Speech-to-text integration
- Integration with emergency dispatch systems
- Larger real-world emergency datasets
- Transformer-based multimodal fusion

---



# 📜 License

This project is created for academic and research purposes.
