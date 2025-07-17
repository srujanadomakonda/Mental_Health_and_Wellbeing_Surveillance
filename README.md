# Mental Health and Wellbeing Surveillance System (MHWSS)

## 📌 Project Overview

The **Mental Health and Wellbeing Surveillance System (MHWSS)** is an IoT- and data-driven framework designed to collect, analyze, and monitor mental health indicators in real time using embedded systems, mobile apps, and cloud integration. It aims to provide early identification of mental health issues, personalized interventions, and collaboration among users, caregivers, and healthcare professionals.


## 🎯 Objectives

- Detect early signs of mental health issues through sensor data and questionnaires.
- Provide personalized support resources like relaxation audio, calorie tracking, and workouts.
- Enable real-time communication between users and mental health professionals.
- Collect and analyze population-level mental health trends using Firebase and ML.

## 🧠 Core Features

- 🧭 **User Registration/Login** (Firebase Auth)
- 📊 **Sensor Data Monitoring**:
  - Heart rate (Pulse Sensor)
  - Physical activity (Accelerometer)
  - Sleep quality (Noise Sensor)
  - Environmental conditions (DHT11, Air Quality Sensor)
- 📱 **Mobile App Functionalities**:
  - Workout and calorie tracking
  - Relaxation audio and sleep support
  - Call support services
  - Mental health quiz
- 🔒 **Data Privacy & Security**:
  - End-to-end encryption
  - Role-based access control
- ☁️ **Cloud Integration**:
  - Real-time data sync with Firebase

## ⚙️ Hardware Used

- 🔌 Arduino UNO (sensor integration)
- 📡 NodeMCU ESP8266 (WiFi & Firebase interface)
- ❤️ Pulse Sensor
- 🌡️ DHT11 Sensor (Temperature & Humidity)
- 🌀 Accelerometer
- 🏭 Air Quality Sensor
- 🔊 Noise Sensor

## 💻 Software Requirements

- Arduino IDE
- Firebase (Realtime Database, Authentication)
- Android Studio (for mobile UI)
- Firebase Libraries (`FirebaseESP8266.h`, etc.)
- MIT App Inventor / Java (for mobile app)

## 🧩 Code Structure

### `FIREBASE_ORIGINAL_FINAL.ino`
- Connects NodeMCU to Firebase via WiFi
- Receives processed sensor data from Arduino over Serial
- Pushes JSON-encoded health parameters to Firebase

### `arduinostructpulse.ino`
- Collects real-time data from sensors
- Processes and structures data
- Sends via Serial to NodeMCU

## 🧪 System Workflow

1. User signs into the app.
2. Arduino collects data from all sensors.
3. NodeMCU reads data via serial and sends it to Firebase.
4. Mobile app retrieves Firebase data to update dashboards.
5. Users receive recommendations based on data (e.g., relaxation sounds, diet tips).
6. Critical thresholds trigger alerts or support calls.


## 📊 Database Schema (Firebase)

- `/users/<user_id>/heart_rate`
- `/users/<user_id>/temperature`
- `/users/<user_id>/activity_level`
- `/users/<user_id>/air_quality`
- `/users/<user_id>/sleep_quality`
- `/alerts/<user_id>`

## 🛡️ Security and Privacy

- Firebase Authentication for user validation
- HTTPS & token-based communication
- Data encryption during transmission
- User consent for data collection

## 📱 App Screens (Highlights)

- Login/Registration
- Main Dashboard
- Workout & Calorie Tracker
- Sleep & Relaxation Audio
- Call Support Services
- Reports & Health Trends


## 🚀 Future Enhancements

- Chatbot for mood tracking and journaling
- Integration with smartwatches for wearable data
- ML-driven risk prediction models
- Anonymous community support chatrooms


## 📚 References

- [CDC Mental Health Surveillance Reports](https://www.cdc.gov/mentalhealth/data_publications/surveillance.html)
- [Firebase Docs](https://firebase.google.com/docs)
- [Arduino Sensor Libraries](https://www.arduino.cc/en/Reference/HomePage)

## 👩‍💻 Contributors

- **Srujana Domakonda**  
  *Project Lead, Code & Documentation*  
  📧 srujanadomakonda@gmail.com


> 💡 This project was developed as part of an academic initiative to leverage embedded systems and cloud computing in public health applications.
