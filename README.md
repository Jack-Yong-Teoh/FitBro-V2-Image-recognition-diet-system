# 🥗 FitBro V2: Intelligent Android Diet System
### *Final Year Project (FYP) - On-Device Image Recognition & Nutritional Analytics*

[![Platform](https://img.shields.io/badge/Platform-Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)](https://www.android.com/)
[![Language](https://img.shields.io/badge/Language-Java%20%2F%20Kotlin-orange?style=for-the-badge&logo=kotlin&logoColor=white)](https://kotlinlang.org/)
[![Machine Learning](https://img.shields.io/badge/AI-TFLite%20%2F%20ML%20Kit-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)](https://www.tensorflow.org/lite)

**FitBro V2** is a native Android application designed to automate the process of nutritional tracking. By utilizing **Computer Vision (TensorFlow Lite)** directly on the mobile device, users can identify food items via the camera and receive instant caloric and macronutrient breakdowns, significantly reducing the friction of manual dieting.

---

## 📌 Problem Statement
Traditional calorie counting apps suffer from high abandonment rates due to the tedious nature of manual logging. FitBro V2 addresses this by implementing an **automated "Snap & Log" workflow**, leveraging on-device machine learning to provide real-time nutritional feedback.

---

## ✨ Key Features
* **📸 Real-Time Food Recognition:** Integrated **CameraX API** with an optimized **TensorFlow Lite (.tflite)** model for instant food classification.
* **📊 Automatic Macro Calculation:** Fetches real-time nutritional data (Calories, Protein, Carbs, Fats) via **Retrofit** integration with the Nutritionix API.
* **📉 Health Metrics Engine:** Personalize goals with built-in **BMI and BMR calculators** based on user profiles.
* **📅 Historical Analytics:** Track dietary trends over time with interactive graphs powered by **MPAndroidChart**.
* **☁️ Data Persistence:** Hybrid storage solution using **Room Database** (local) and **Firebase** (cloud) for seamless data syncing.

---

## 🏗️ Technical Architecture
The project is built using the **MVVM (Model-View-ViewModel)** architectural pattern, ensuring a clean separation of concerns and a robust foundation for an FYP.

* **View:** XML-based layouts with Material Design components.
* **ViewModel:** Handles UI logic and maintains state during configuration changes.
* **Repository:** Orchestrates data flow between the **Local Room DB** and the **Remote API**.
* **AI Engine:** Processes image frames through a **Convolutional Neural Network (CNN)** optimized for mobile hardware acceleration (NNAPI).

---

## 🛠️ Tech Stack & Libraries

| Category | Tools / Libraries |
| :--- | :--- |
| **Development Environment** | Android Studio (Java/Kotlin) |
| **Networking** | Retrofit 2, OkHttp, GSON |
| **Image Loading** | Glide / Picasso |
| **Machine Learning** | TensorFlow Lite, ML Kit, CameraX |
| **Database** | Room Persistence, Firebase Realtime DB |
| **UI Components** | Material Components, MPAndroidChart |

---

## 🚀 Getting Started

To explore or build the FitBro V2 project:

### 1. Prerequisites
* Android Studio (Ladybug 2024.2.1 or later recommended).
* Android Device with Camera (API Level 21+).
* Nutritionix API Key (for nutritional data fetching).

### 2. Installation
1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/Jack-Yong-Teoh/FitBro-V2-Image-recognition-diet-system.git
    ```
2.  **Import to Android Studio:**
    `File > Open > [Project Folder]`
3.  **Gradle Sync:**
    Wait for the IDE to finish syncing the dependencies defined in `build.gradle`.
4.  **Configuration:**
    Place your `google-services.json` in the `app/` folder (if using Firebase) and add your API keys to the `Constants` file.
5.  **Run:**
    Connect your device and click the **Run** button.

---

## 🔬 AI Methodology
The food recognition component utilizes **Transfer Learning** to classify 100+ food categories.
* **Model Optimization:** The model is quantized to **FP16/INT8** to ensure low-latency inference on mid-range Android hardware.
* **Image Processing:** Custom `ImageAnalyzer` implementation using CameraX to pipe frames directly into the TFLite interpreter.

---

## 👤 Author
**Jack Yong Teoh**
* **GitHub:** [@Jack-Yong-Teoh](https://github.com/Jack-Yong-Teoh)
* **Project Link:** [FitBro-V2-Android](https://github.com/Jack-Yong-Teoh/FitBro-V2-Image-recognition-diet-system)

---
*Developed as a Final Year Project (FYP). Undergrad Research into Mobile AI and Digital Health.*
