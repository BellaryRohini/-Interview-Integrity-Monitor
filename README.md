# 🛡️ Interview Integrity Monitor

> 🚀 A zero-install web application that helps recruiters identify possible AI-assisted cheating during remote interviews.

---

## 📌 Overview

Interview Integrity Monitor detects **behavioral signals** that may indicate AI-assisted interview cheating without installing any software on the candidate's computer.

Instead of detecting specific AI tools, it analyzes multiple signals and provides a **risk score** along with clear evidence for a human reviewer.

> ⚠️ This system is designed to **assist recruiters**, not automatically reject candidates.

---

## ✨ Features

- 🎧 Virtual Audio Device Detection
- ⏱️ Response Delay Analysis
- 🎤 Speech Recognition & Transcription
- 💬 Filler Word Analysis
- 👀 Eye Movement Analysis (MediaPipe)
- 📊 Risk Score (Low / Medium / High)
- 📋 Recruiter-Friendly Dashboard
- 📥 Download Session Report (JSON)
- 📈 Calibration Tool for Threshold Tuning

---

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| 🌐 HTML | User Interface |
| 🎨 CSS | Styling |
| ⚡ JavaScript | Detection Logic |
| 👁️ MediaPipe Face Landmarker | Eye Tracking |
| 🎙️ Web Speech API | Speech Recognition |
| 🐍 Python | Calibration Tool |
| 📊 Matplotlib | Session Analysis |

---

## 📂 Project Structure

```text
Interview-Integrity-Monitor/
│
├── 📄 index.html
├── 🐍 analyze_sessions.py
├── 📘 README.md
├── 📦 requirements.txt
├── 📁 sample_sessions/
└── 📁 screenshots/
```

---

## ⚙️ Installation

### 1️⃣ Clone the Repository

```bash
git clone <repository-url>
```

### 2️⃣ Open the Project

```bash
cd Interview-Integrity-Monitor
```

### 3️⃣ Create a Virtual Environment

```bash
python -m venv venv
```

### 4️⃣ Activate the Environment

**Windows**

```bash
.\venv\Scripts\activate
```

### 5️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Run the Application

Start a local web server

```bash
python -m http.server 8000
```

Open your browser and visit

```
http://localhost:8000
```

> 💡 For the best experience, use **Google Chrome**, as the application relies on the Web Speech API.

---

## 🔍 Detection Signals

The system combines multiple signals to estimate interview integrity:

- 🎧 Virtual Audio Device Detection
- ⏱️ Response Latency Analysis
- 💬 Speech Pattern Analysis
- 👀 Eye Movement Detection

These signals are combined into a **risk score** instead of making a binary decision.

---

## 📊 Risk Levels

| Level | Meaning |
|------|---------|
| 🟢 Low | No significant suspicious activity |
| 🟡 Medium | Some suspicious behavior detected |
| 🔴 High | Multiple signals suggest possible AI assistance |

---

## 📈 Calibration Tool

Analyze collected interview sessions using:

```bash
python analyze_sessions.py sample_sessions
```

The tool generates:

- 📊 Signal distributions
- 📉 Threshold suggestions
- 🖼️ Calibration charts

---

## 🚧 Limitations

- ❌ Does not identify specific AI tools by name.
- 📱 Cannot detect off-camera devices such as phones or another laptop.
- 🤝 Does not automatically reject candidates.
- 👨‍💼 Results are intended to support human reviewers.

---

## 🚀 Future Improvements

- 📄 PDF Report Generation
- 📡 Real-Time Recruiter Dashboard
- 🤖 Adaptive Threshold Calibration
- 📊 Recruiter Analytics
- ☁️ Cloud Deployment

---

## 📜 License

Developed as part of the **🏆 InCruiter – Catch the Invisible AI Cheater Hackathon**.

---

## ⭐ If you found this project useful, consider giving it a star!
