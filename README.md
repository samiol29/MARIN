# M.A.R.I.N. — Marine AI Recognition & Identification Network

<div align="center">

### Embedded Intelligent Microscopy System for Identification & Counting of Microscopic Marine Organisms

**Smart India Hackathon 2025 (SIH 2025)**

AI-Powered Marine Microscopy • Edge Intelligence • Real-Time Biodiversity Analytics

</div>

---

# Overview

M.A.R.I.N. (Marine AI Recognition & Identification Network) is an embedded AI-powered intelligent microscopy system developed for **Smart India Hackathon 2025** under Problem Statement ID **25043**.

The system is designed to automate the identification and counting of microscopic marine organisms using:
- embedded edge computing,
- computer vision,
- TensorFlow Lite inference,
- microscopy imaging,
- and real-time biodiversity analytics.

MARIN combines:
- Raspberry Pi-based edge inference,
- microscopic image acquisition,
- lightweight AI models,
- sensor-assisted sample management,
- and a MERN-based analytics dashboard

into a scalable marine biodiversity intelligence platform.

---

# Problem Statement

Marine researchers and ocean monitoring agencies face several critical challenges during microscopic marine organism analysis:

## Massive Data Backlog
Manual microscopy analysis is time-consuming and slows biodiversity research.

## Inconsistent Manual Counting
Human counting errors create unreliable datasets and inconsistent observations.

## Environmental Change
Marine samples may become outdated before complete analysis is performed.

Traditional laboratory workflows:
- require skilled manual inspection,
- lack automation,
- are expensive to scale,
- and cannot efficiently process large biodiversity datasets.

---

# Solution

MARIN introduces an AI-assisted embedded microscopy platform capable of:

- Capturing microscopic water-sample imagery
- Running real-time organism detection on edge devices
- Automatically identifying and counting marine organisms
- Displaying instant results on LCD interfaces
- Aggregating biodiversity data into analytics dashboards
- Supporting large-scale marine biodiversity monitoring

The system provides:
- faster analysis,
- reduced manual effort,
- improved counting consistency,
- and scalable marine intelligence workflows.

---

# Core Innovation

The uniqueness of MARIN lies in the integration of:

| Domain | Contribution |
|---|---|
| Embedded Systems | Edge AI deployment |
| Computer Vision | Microscopic image analysis |
| Deep Learning | Organism identification |
| Edge Computing | Real-time onboard inference |
| MERN Stack | Biodiversity analytics dashboard |
| Marine Research | Automated microscopy workflows |

Rather than functioning as a standalone ML notebook, MARIN was designed as a deployable intelligent marine microscopy ecosystem.

---

# System Architecture

```text
                ┌──────────────────────────┐
                │ Water Sample Collection  │
                └────────────┬─────────────┘
                             │
                             ▼
                ┌──────────────────────────┐
                │ Pi Camera Microscopy     │
                │ Image Capture            │
                └────────────┬─────────────┘
                             │
                             ▼
                ┌──────────────────────────┐
                │ Raspberry Pi 5           │
                │ Edge AI Inference        │
                │ TensorFlow Lite Model    │
                └────────────┬─────────────┘
                             │
           ┌─────────────────┼─────────────────┐
           ▼                 ▼                 ▼
  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐
  │ LCD Results  │  │ JSON Output  │  │ Barcode/     │
  │ Display      │  │ Serialization│  │ Voice Notes  │
  └──────────────┘  └──────┬───────┘  └──────────────┘
                            │
                            ▼
                ┌──────────────────────────┐
                │ Node.js + Express API    │
                └────────────┬─────────────┘
                             │
                             ▼
                ┌──────────────────────────┐
                │ MongoDB Aggregation      │
                │ Biodiversity Analytics   │
                └────────────┬─────────────┘
                             │
                             ▼
                ┌──────────────────────────┐
                │ React Dashboard          │
                │ Chart.js Visualization   │
                └──────────────────────────┘
```

---

# Hardware Components

## Raspberry Pi 5 (8GB)
Primary edge compute device responsible for:
- image processing,
- AI inference,
- local computation,
- and device orchestration.

### Specifications
- ARM Cortex-A76 CPU
- Edge AI execution
- Real-time processing support

---

## Raspberry Pi Camera Module 3

Used for:
- microscopic image acquisition,
- real-time sample capture,
- organism visualization.

Connected via:
- MIPI CSI interface.

---

## SPI LCD Display

Provides:
- instant visual results,
- organism counts,
- edge inference feedback,
- local monitoring interface.

---

## Environmental Sensors

Additional marine sensing support includes:
- pH Sensor
- Turbidity Sensor
- Optical Density Sensor

These sensors assist in:
- environmental condition analysis,
- sample monitoring,
- and biodiversity correlation.

---

## Communication & Networking

The Raspberry Pi uses:
- Wi-Fi
- Ethernet

for:
- dashboard synchronization,
- JSON transmission,
- cloud/backend communication.

---

# AI & Deep Learning Pipeline

The AI engine of MARIN uses lightweight CNN-based computer vision models optimized for edge deployment.

The system:
1. captures microscopic frames,
2. preprocesses imagery,
3. runs TensorFlow Lite inference,
4. identifies microscopic organisms,
5. counts detected organisms,
6. serializes outputs,
7. and transmits results for aggregation.

---

# Why TensorFlow Lite?

TensorFlow Lite was selected because:
- it is optimized for edge devices,
- supports low-latency inference,
- reduces memory usage,
- and performs efficiently on Raspberry Pi hardware.

This enables:
- real-time organism detection,
- lightweight deployment,
- and portable marine analysis systems.

---

# Workflow

## Step 1 — Sample Capture
Microscopic water samples are captured using:
- Raspberry Pi Camera Module 3.

---

## Step 2 — Edge Inference
Raspberry Pi 5 executes:
- TensorFlow Lite AI inference
- microscopic organism detection
- counting & classification.

---

## Step 3 — LCD Visualization
Inference results are instantly displayed on:
- SPI LCD Display.

---

## Step 4 — Data Serialization
Detection outputs are packaged into:
- structured JSON payloads.

---

## Step 5 — Backend Aggregation
Node.js + Express APIs:
- receive organism data,
- process logs,
- and store biodiversity analytics in MongoDB.

---

## Step 6 — Dashboard Analytics
React + Chart.js frontend visualizes:
- biodiversity metrics,
- temporal analysis,
- organism trends,
- and ecosystem insights.

---

# Tech Stack

## Artificial Intelligence & Computer Vision

| Technology | Purpose |
|---|---|
| TensorFlow Lite | Edge AI inference |
| OpenCV | Image preprocessing |
| Python | AI pipeline |
| CNN Models | Organism classification |

---

## Frontend

| Technology | Purpose |
|---|---|
| React.js | Dashboard frontend |
| Chart.js | Biodiversity visualization |
| HTML/CSS/JavaScript | UI development |

---

## Backend

| Technology | Purpose |
|---|---|
| Node.js | Backend runtime |
| Express.js | API services |
| MongoDB | Biodiversity data storage |

---

## Embedded Hardware

| Hardware | Purpose |
|---|---|
| Raspberry Pi 5 | Edge AI compute |
| Pi Camera 3 | Microscopy image capture |
| LCD Display | Local result display |
| Environmental Sensors | Marine condition analysis |

---

# Key Features

## Real-Time Organism Identification
AI-assisted microscopic analysis directly on edge hardware.

## Automated Counting
Removes inconsistencies caused by manual counting workflows.

## Edge Intelligence
Inference performed locally on Raspberry Pi without dependency on cloud computation.

## Biodiversity Dashboard
Interactive MERN dashboard for analytics and long-term monitoring.

## Voice Annotation Support
Researchers can attach voice-based observations using speech-to-text integration.

## Sample Management System
Barcode/sample tagging support for research workflows.

---

# Innovation Highlights

## Embedded AI Microscopy
Combines microscopy and edge AI into one portable marine analysis system.

## Lightweight Edge Inference
Uses TensorFlow Lite models optimized for Raspberry Pi deployment.

## Marine Biodiversity Intelligence
Supports scalable biodiversity tracking and ecosystem analysis.

## Smart Research Workflow Integration
Designed to integrate into existing marine biology research processes.

---

# Feasibility & Viability

## Strengths
- Portable and low-cost alternative to laboratory systems
- Real-time microscopic analysis
- Fast biodiversity monitoring
- AI-assisted automation
- MERN-based scalable analytics

## Challenges
- Limited labeled marine datasets
- Harsh marine deployment conditions
- Edge-device inference constraints

## Mitigation Strategies
- Transfer learning on plankton datasets
- Lightweight optimized AI models
- Rugged hardware enclosures
- Incremental MVP scaling

---

# Potential Applications

## Marine Research & Biology
- organism identification
- biodiversity monitoring
- plankton analysis

## Environmental Monitoring
- ecosystem health tracking
- marine condition analysis
- aquatic biodiversity studies

## Fisheries & Aquaculture
- harmful organism detection
- sustainable aquaculture monitoring

## Educational & Research Institutions
- affordable AI microscopy platform
- marine biology learning tool

---

# Future Roadmap

## AI Improvements
- Advanced transfer learning
- Multi-organism classification
- Object detection models (YOLO)
- Real-time segmentation systems

## Hardware Expansion
- Rugged marine deployment systems
- Autonomous sampling units
- Waterproof field enclosures

## Platform Expansion
- Cloud synchronization
- Mobile dashboard support
- Real-time biodiversity alerts
- Multi-device marine intelligence networks

---

# Repository Structure

```text
MARIN/
│
├── marin-cnn-model2.ipynb
├── backend/
├── frontend/
├── dataset/
├── outputs/
├── models/
├── images/
├── README.md
└── requirements.txt
```

---

# Setup Instructions

## Clone Repository

```bash
git clone <repository-url>
cd MARIN
```

---

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Run Notebook

```bash
jupyter notebook
```

Open:

```text
marin-cnn-model2.ipynb
```

and execute cells sequentially.

---

# Contributors

Developed as part of **Smart India Hackathon 2025**

Team SANAM

- Anshukman MJ
- Adithi Netra S
- Ashikka R B
- Nitish M
- Shyaam Karodiya
- Mrithul Samuel S

---

# License

MIT License © 2025 MARIN
```
