<div align="center">

# ❤️ Heart Disease Prediction

*An End-to-End Machine Learning Web Application for Heart Disease Detection.*

[![Python Version](https://img.shields.io/badge/Python-3.9+-3776AB?style=flat&logo=python)](https://www.python.org/)
[![Framework: Flask](https://img.shields.io/badge/Framework-Flask-black?style=flat&logo=flask)](https://flask.palletsprojects.com/)
[![Docker](https://img.shields.io/badge/Docker-Enabled-2496ED?style=flat&logo=docker)](https://www.docker.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

</div>

---

**Heart Disease Prediction** is a machine learning project built to detect heart disease from simple physical test inputs. It features a complete pipeline from data ingestion and hyperparameter tuning to a Flask-based web application and containerized Docker deployment.

## 📑 Table of Contents

- [Features](#-features)
- [Technology Stack](#-technology-stack)
- [Getting Started](#-getting-started)
  - [Prerequisites](#prerequisites)
  - [Local Setup](#local-setup)
  - [Docker Setup](#docker-setup)
- [Usage](#-usage)
- [User Interface](#️-user-interface)
- [License](#-license)

---

## ✨ Features

- **End-to-End ML Pipeline:** Includes distinct phases for research, data ingestion, data preprocessing, data transformation, model building, and hyperparameter tuning.
- **Interactive Web Interface:** A sleek UI served via Flask to collect patient features and return real-time predictions.
- **Predictive Power:** Evaluates physical features (Age, Sex, ChestPainType, Cholesterol, FastingBS, MaxHR, ExerciseAngina, Oldpeak, ST_Slope) to predict if heart disease is present or absent.
- **Containerized:** Fully Dockerized setup for simple and consistent deployment across all environments.

---

## 🚀 Technology Stack

| Domain | Technologies |
| :--- | :--- |
| **Backend/Web** | Python 3.9, Flask |
| **Machine Learning**| Scikit-learn (1.3.2), XGBoost |
| **Data Processing** | Pandas, Numpy, Seaborn |
| **Deployment** | Docker |

---

## 🏁 Getting Started

Follow these instructions to get a copy of the project up and running on your local machine for development and testing.

### Prerequisites

Ensure you have the following installed:
- [Python](https://www.python.org/downloads/) (3.9+)
- [Git](https://git-scm.com/downloads/)
- [Docker](https://docs.docker.com/get-docker/) (Optional, for containerized execution)

### Local Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/aashaybelekar/HeartDiseasePrediction.git
   cd HeartDiseasePrediction
   ```

2. **Install Python Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Application:**
   ```bash
   python app.py
   ```

### Docker Setup

1. **Build the Docker Image:**
   The application is containerized using the official Python 3.9-slim image.
   ```bash
   docker build -t heart-disease-app .
   ```
   *Note: The Dockerfile automatically installs dependencies from `requirements.txt` and configures the local project as a dependency.*

2. **Run the Container:**
   ```bash
   docker run -p 5000:5000 heart-disease-app
   ```
   *The container runs the Flask application using the `FLASK_APP=app.py` environment variable.*

---

## ▶️ Usage

Once the application is running locally or via Docker, open your web browser and navigate to:  
`http://127.0.0.1:5000/`

1. **Home Page (`/`):** Provides an overview of the application.
2. **Predict Data Endpoint (`/predictdata`):** Fill out the HTML form with patient metrics to receive an instant prediction on whether heart disease is likely present or absent.

---

## 🖼️ User Interface

### Video Demo
[![Watch the video](https://raw.githubusercontent.com/aashaybelekar/HeartDiseasePrediction/main/images/VideoThumb.png)](https://youtu.be/9f9krzL4piA)

### Home page
![Home Page](https://raw.githubusercontent.com/aashaybelekar/HeartDiseasePrediction/main/images/homepage.png)

### Form
![Form](https://raw.githubusercontent.com/aashaybelekar/HeartDiseasePrediction/main/images/form.jpg)

---

## 📝 License

This project is open-source and available under standard open-source terms.
