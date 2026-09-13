# KitaBisa — Sign Language Learning Platform

KitaBisa is an interactive web-based platform designed to help users learn and practice sign language through **learning materials, quizzes, AI-powered webcam practice, and an online community**.

The platform combines web development and artificial intelligence to provide an engaging learning experience while allowing users to track their learning progress through scores and performance records.

## ✨ Features

### 📚 Learning

Users can learn sign language through structured learning materials and visual references.

* Sign language learning materials
* Visual examples for different signs
* Beginner-friendly learning interface
* Organized learning content

### 🧠 AI-Powered Sign Language Practice

KitaBisa provides an AI-based practice feature that allows users to practice sign language using their webcam.

The system analyzes the user's hand gestures and provides a score based on the detected sign.

**Practice flow:**

```text
Webcam
   ↓
Hand Tracking
   ↓
AI Model
   ↓
Sign Prediction
   ↓
Score / Feedback
   ↓
Progress Tracking
```

The AI component runs through a **FastAPI backend**, which handles communication between the web application and the machine learning model.

### 📝 Quiz

Users can test their understanding through interactive quizzes.

* Practice questions
* Score calculation
* Learning assessment
* Progress tracking

### 📊 Progress Tracking

KitaBisa records user performance to help users monitor their learning progress.

Users can track:

* Quiz scores
* AI practice scores
* Learning performance
* Overall progress

This allows users to identify areas where they need more practice.

### 👥 Online Community

KitaBisa includes an online community where users can interact and share their learning experiences.

Users can:

* Share posts
* Discuss sign language
* Interact with other learners
* Share their learning experiences

The community is designed to make learning more interactive and collaborative.

---

## 🏗️ System Architecture

KitaBisa uses a web application architecture with a Django application and a separate AI service.

```text
                    ┌─────────────────────┐
                    │      Web Browser     │
                    │                     │
                    │  Learning / Quiz    │
                    │  Community / Webcam │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │   Django Backend    │
                    │                     │
                    │ Users / Learning    │
                    │ Quiz / Community    │
                    │ Progress Tracking   │
                    └──────────┬──────────┘
                               │
                               │ AI Requests
                               ▼
                    ┌─────────────────────┐
                    │   FastAPI Backend   │
                    │                     │
                    │ AI Model Inference  │
                    │ Hand Detection      │
                    │ Sign Prediction     │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │    AI / ML Model    │
                    │                     │
                    │ Hand Gesture        │
                    │ Recognition         │
                    └─────────────────────┘
```

---

## 🛠️ Tech Stack

### Frontend

* HTML
* CSS
* JavaScript

### Backend

* Django
* FastAPI
* REST API / WebSocket communication

### Artificial Intelligence

* Python
* TensorFlow
* MediaPipe
* Computer Vision
* Hand Tracking
* Machine Learning

### Database

* Django Database System

---

## 📁 Project Structure

```text
KitaBisa/
│
├── base/
│   └── ...
│
├── djangoProject3/
│   ├── ...
│   └── Django application
│
├── pythonmodel/
│   ├── ...
│   └── AI / machine learning components
│
├── manage.py
│
└── README.md
```

---

## 🚀 How It Works

### 1. Learning

Users access the learning section and study different sign language gestures using the available learning materials.

### 2. Quiz

After learning the material, users can complete quizzes to evaluate their understanding.

### 3. AI Practice

Users can switch to AI practice mode and enable their webcam.

The AI system detects the user's hand movements and predicts the performed sign.

### 4. Scoring

The AI practice system evaluates the user's performance and generates a score.

The score is then used as feedback for the user.

### 5. Progress

Quiz and practice results can be used to monitor the user's overall learning progress.

---

## 🎯 Project Goals

KitaBisa was developed with several goals:

* Make sign language learning more accessible
* Provide an interactive way to practice sign language
* Use AI to provide real-time practice feedback
* Encourage consistent learning through progress tracking
* Create an online community for learners
* Combine education, artificial intelligence, and web technology into one platform

---

## 💡 Why KitaBisa?

Traditional learning methods may not provide immediate feedback when someone practices sign language.

KitaBisa addresses this by combining **learning materials, quizzes, AI-powered webcam practice, and progress tracking** in one platform.

Instead of only learning what a sign looks like, users can directly practice the gesture and receive a score from the AI system.

---

## 🔮 Future Improvements

Potential future improvements include:

* Support for more sign language gestures
* Improved AI recognition accuracy
* More advanced performance analytics
* Personalized learning recommendations
* Gamification and achievement systems
* Real-time community interaction
* Mobile application support
* More detailed AI feedback for incorrect gestures

---

## 👨‍💻 Project

**KitaBisa**
An AI-powered sign language learning platform combining web development, machine learning, and interactive education.

---

## 📄 License

This project is intended for educational and development purposes.
