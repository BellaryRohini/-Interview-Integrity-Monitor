# Interview Integrity Monitor

## Overview

Interview Integrity Monitor is a zero-install web application that helps recruiters identify possible AI-assisted cheating during online interviews.

Instead of detecting specific AI tools, it analyzes behavioral signals that may indicate external assistance and presents the findings to a human reviewer.

---

## Features

- Virtual audio device detection
- Response delay analysis
- Speech transcription
- Filler-word analysis
- Eye movement analysis using MediaPipe
- Risk scoring (Low / Medium / High)
- Recruiter-friendly dashboard
- Downloadable JSON session report
- Threshold calibration tool

---

## Tech Stack

- HTML
- CSS
- JavaScript
- MediaPipe Face Landmarker
- Web Speech API
- Python
- Matplotlib

---

## Project Structure

```
Interview-Integrity-Monitor/
│
├── index.html
├── analyze_sessions.py
├── README.md
├── requirements.txt
└── sample_sessions/
```

---

## Installation

Clone the repository

```bash
git clone <repository-url>
```

Go to the project folder

```bash
cd Interview-Integrity-Monitor
```

Create a virtual environment

```bash
python -m venv venv
```

Activate the virtual environment

Windows

```bash
.\venv\Scripts\activate
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

## Run the Project

Start a local server

```bash
python -m http.server 8000
```

Open

```
http://localhost:8000
```

Use Google Chrome for the best experience because the application uses the Web Speech API.

---

## Calibration

To analyze collected interview sessions, run

```bash
python analyze_sessions.py sample_sessions
```

This generates calibration statistics and charts for tuning detection thresholds.

---

## Detection Signals

- Virtual audio devices
- Response latency
- Speech patterns
- Eye movement patterns

The application combines multiple signals into a risk score rather than relying on a single indicator.

---

## Limitations

- Does not detect specific AI tools by name.
- Cannot detect a second phone or another off-camera device.
- Does not automatically reject candidates.
- Results should always be reviewed by a human.

---

## Future Improvements

- Adaptive threshold calibration
- Additional behavioral signals
- Recruiter analytics dashboard
- PDF report generation

---

## License

This project was developed as part of the **InCruiter Interview Integrity Hackathon**.
