# 🌱 Project-OnlyPlants

> **Cloud-based IoT and AI dashboard for precision agriculture of orchids.**

---
## 👥 Team Members
* **Linoy Cohen** 
* **Tehila Ben Dahan** 
* **Yarden Ben Shitrit** 
* **Yuval Rotenberg** 

---
## 📖 About the Project
A smart, cloud-based system tailored specifically for orchid growers. The application provides a professional dashboard to monitor, analyze, and control plant health in real-time, integrating advanced AI analysis and IoT sensor data along with engaging gamification features to elevate the user experience.

## 🏗️ Architecture Explanation 
The OnlyPlants system is designed using a **Microservices Architecture**. The application is divided into small, independent services (IoT Ingestion, AI Image Processing, Gamification Engine, and User Dashboard). This modularity allows us to scale services independently—for example, scaling up the AI service during peak image upload times without affecting the IoT sensor data stream. Inter-service communication is handled via REST APIs and event queues.

## 🔌 Services Documentation 
* **User Service:** Manages user profiles, authentication, and the Gamification points/leaderboards.
* **IoT Dashboard Service:** Receives, formats, and displays real-time telemetry from environmental sensors (moisture, light, temperature).
* **AI Analysis Service:** Accepts image uploads, processes them through our trained models to detect orchid diseases, and returns actionable insights.

## 🚀 Usage Examples 
* **Planting a new Orchid:** User logs in, registers a new plant, and connects the corresponding IoT sensor MAC address.
* **Health Check:** User uploads a photo of a yellowing leaf. The AI Analysis Service processes it and returns: `{"status": "disease_detected", "disease": "Crown Rot", "confidence": 92%}`.
* **Gamification:** Completing a daily task (e.g., watering based on IoT alert) triggers the User Service to award +50 points to the user's profile.

## ✅ Test Results 
* **Unit Tests:** Successfully passed unit tests for ranking mechanisms and AND/OR logical operators in the query algorithms.
* **Load Testing:** Verified the system handles 500 concurrent simulated IoT sensor updates per minute with a response time of < 1.5 seconds.

## ✨ Key Features
* 📸 **AI Image Analysis:** Automated disease identification, moisture stress evaluation, and pest detection based on images.
* 🌡️ **Real-Time IoT Monitoring:** Continuous stream of environmental data (temperature, soil moisture, and light intensity) from remote sensors.
* 📊 **Visual Dashboard:** Interactive charts showing plant history, live health metrics, trends, and behavioral comparisons.
* 🎮 **Gamification Elements:** Daily maintenance missions, a reward point system, weekly challenges, and a community leaderboard to promote best care practices.

---

## 📓 Tutorial Notebooks (Google Colab Links)
Here are the linear notebook links for the lab sessions and exercises conducted throughout the course. Click on any link below to open and run the code directly in Google Colab:

* **Tutorial 1** https://colab.research.google.com/drive/1BZtrIiJZeeHxYt5crdjm3sLfeH6jBKNw?usp=sharing
* **Tutorial 2** https://colab.research.google.com/drive/1GVmaLEtSUy5v_eYAfBdOWXxLPBqbVwMu?usp=sharing
* **Tutorial 3** https://colab.research.google.com/drive/1nxDkwa9XqUay-xcDhuKSXxcvAPr75YHt?usp=sharing
* **Tutorial 4** https://colab.research.google.com/drive/10f89GSQi9c_oDNtWBI_SCDvzPcwKDX4q?usp=sharing
* **Tutorial 5** https://colab.research.google.com/drive/1PjkXzaIXWEyA3PsJK_ii_JbqFPhQFmek?usp=sharing
* **Tutorial 6** https://colab.research.google.com/drive/1hpfcev65HLmkF4pAsml-WFLHS4Yv2dEo?usp=sharing
* **Tutorial 7** https://colab.research.google.com/drive/14I8f3cxyvi0BdhCCKlMvyQnyUnrkOjEY?usp=sharing

