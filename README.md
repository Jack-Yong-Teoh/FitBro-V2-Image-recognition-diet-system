# 🥗 FitBro V2: Intelligent Image-Recognition Diet System
### *Final Year Project (FYP) - Revolutionizing Nutritional Tracking with Computer Vision*

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/Backend-Python%20%2F%20FastAPI-blue.svg)](#)
[![Computer Vision](https://img.shields.io/badge/AI-YOLOv8%20%2F%20TensorFlow-orange.svg)](#)
[![Mobile](https://img.shields.io/badge/Mobile-React%20Native%20%2F%20Flutter-61dafb.svg)](#)

**FitBro V2** is an AI-powered fitness companion designed to bridge the gap between dietary goals and manual logging fatigue. By leveraging state-of-the-art **Computer Vision**, FitBro allows users to simply snap a photo of their meal to receive an instant breakdown of calories and macronutrients.

---

## 📌 Problem Statement
Manual calorie counting is the #1 reason users abandon diet apps. Traditional logging requires searching through massive databases, weighing portions, and manual entry. FitBro V2 aims to reduce this friction by automating the identification process through AI.



## ✨ Key Features
* **📸 AI Food Recognition:** snap a photo to identify food items automatically using deep learning models.
* **📊 Real-time Macro Analysis:** Instant calculation of Calories, Protein, Carbs, and Fats.
* **📈 Personalized Fitness Goals:** Dynamic calorie targets based on BMI, BMR, and activity levels.
* **📅 Progress Analytics:** Visualized weekly and monthly reports on nutritional trends.
* **💾 Cloud Persistence:** Securely sync logs and user profiles across multiple devices.

---

## 🏗️ System Architecture



FitBro V2 utilizes a **Microservices-inspired architecture**:
1.  **Client Layer:** Mobile application for user interaction and image capture.
2.  **AI Engine:** A specialized Python service running **YOLO** (You Only Look Once) for object detection.
3.  **Core API:** Manages user authentication, business logic, and third-party nutritional API integrations.
4.  **Data Layer:** Persistent storage for user metrics and historical logs.

---

## 🛠️ Tech Stack

| Category | Technologies |
| :--- | :--- |
| **Frontend** | React Native / Flutter |
| **Backend** | Python (FastAPI / Flask) |
| **Machine Learning** | YOLOv8, TensorFlow Lite, OpenCV |
| **Database** | MongoDB / Firebase |
| **APIs** | Nutritionix API, Google Vision API |

---

## 🚀 Local Setup

Follow these steps to get your development environment running:

### 1. Clone the repository
```bash
git clone https://github.com/Jack-Yong-Teoh/FitBro-V2-Image-recognition-diet-system.git
cd FitBro-V2-Image-recognition-diet-system
