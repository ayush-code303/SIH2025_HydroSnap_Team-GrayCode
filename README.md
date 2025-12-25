<div align="center">

![License](https://img.shields.io/github/license/mohsinansari0705/SIH2025-HydroSnap)
![Build](https://img.shields.io/github/actions/workflow/status/mohsinansari0705/SIH2025-HydroSnap/ci.yml?label=Build)
![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)
![Tech](https://img.shields.io/badge/Made%20with-Android%20%7C%20FastAPI%20%7C%20Postgres%20%7C%20OpenCV-blue)

# 🌊 HydroSnap – Secure River Water Level Monitoring

<img src="assets/icons/HydroSnap_logo.png" alt="HydroSnap Application logo" heigt=500 width=500>

</div>

## NOTE: 
ITS A SAMPLE COPY OF OUR FINAL WORK ON SIH 2025 PROJECT FOR PROOF AND VERIFICATION PURPOSE ONLY, NOT FOR COMMERCIAL USE. PLEASE DO NOT USE ANY CONTENT WITHOUT PERMISSION FROM THE ORIGINAL AUTHORS (TEAM - GRAYCODE).

---

## 📌 Overview
**HydroSnap** is a mobile-first solution to modernize and secure **river water-level monitoring** using **image processing, geofencing, and cloud integration**.  
It provides reliable, tamper-proof, and scalable data collection to support **flood forecasting, disaster preparedness, and water resource management**.  

---

## 🚩 Problem Statement
Water levels in rivers across India are still largely **monitored manually** by field personnel.  
This process is **time-consuming, error-prone, and vulnerable to tampering**.  

---

## 💡 Our Solution
HydroSnap ensures **authentic and secure water-level reporting** by combining:  
✅ GPS-based **geofencing** for site validation  
✅ **QR code verification** for site authenticity  
✅ **Live photo capture** of gauge posts (no gallery uploads)  
✅ **Image Processing (OCR/AI)** to read water levels automatically  
✅ **Metadata tagging** – timestamp, GPS coordinates, device ID, user ID  
✅ **Tamper detection** – anomaly detection for fake/duplicate readings  
✅ **Offline-first sync** for remote/rural areas  
✅ **Dashboard integration** for supervisors & central analysts  

---

## ✨ Features
- 🌍 **Location Validation** – Warns if user is outside monitoring site radius.  
- 📷 **Camera Enforcement** – Captures live image for each reading.  
- 🤖 **AI Assistance** – Detects & suggests water level from gauge photo.  
- 🛰️ **Metadata Traceability** – Stores GPS, timestamp, and device ID.  
- 📡 **Offline Mode** – Readings saved locally & synced when online.  
- 👥 **Role-based Access** – Field staff, supervisors, analysts, public.  
- 🔒 **Tamper Detection** – Alerts for skipped/fake readings or GPS spoofing.  
- 📊 **Readings Dashboard** – Supervisors track data across multiple sites.  

---

## 🏗️ Tech Stack
**Mobile (Android)**: Kotlin, Jetpack Compose, CameraX, Room, ZXing (QR Scanner)  
**Backend**: FastAPI / Node.js, REST APIs, JWT Auth  
**Database**: PostgreSQL + PostGIS, Cloud Object Storage (S3/GCS/Azure)  
**Image Processing**: OpenCV, Tesseract OCR, ML (YOLO/CRNN for gauge reading)  
**Dashboard**: React, Mapbox/Leaflet, TailwindCSS    

---

## 📊 Workflow
```mermaid
flowchart TD
    A[User Login & Role Authentication] --> B[Site Verification]
    B -->|GPS Geofence| C[QR Code Scan]
    C --> D[Data Capture]
    D -->|Live Camera + OCR| E[Metadata Tagging]
    E --> F[Offline Storage]
    F --> G[Server Sync & Validation]
    G --> H[Tamper Detection & Alerts]
    H --> I[Supervisor Dashboard]
    I --> J[Central Analysis & Forecasting]
```

---

## 👥 Team: GrayCode

| Name            | Role                          |
|-----------------|-------------------------------|
| [`Mohsin Ansari`](https://github.com/mohsinansari0705)   | Model Integration & Backend |
| [`Rohit Yadav`](https://github.com/RohityadavGG)     | Data & Visualizations       |
| [`Ayush`](https://github.com/ayush-code303)     | Backend Development       |
| [`Prerna Verma`](https://github.com/prerna-verma29)     | UI/UX       |
| [`Payal Katara`](https://github.com/Payal-katara)     | UI/UX & R&D       |
| [`Kunal Singh`](https://github.com/Kunal-Singh76)     | Testing & Reporting       |

---