### Network Security Projects For Phising Data

Setup github secrets:
AWS_ACCESS_KEY_ID=

AWS_SECRET_ACCESS_KEY=

AWS_REGION = us-east-1

AWS_ECR_LOGIN_URI = 788614365622.dkr.ecr.us-east-1.amazonaws.com/networkssecurity
ECR_REPOSITORY_NAME = networkssecurity


Docker Setup In EC2 commands to be Executed
#optinal

sudo apt-get update -y

sudo apt-get upgrade

#required

curl -fsSL https://get.docker.com -o get-docker.sh

sudo sh get-docker.sh

sudo usermod -aG docker ubuntu

newgrp docker


# 🛡️ Network Security ML — Phishing Detection

An end-to-end **Machine Learning project for detecting phishing-related network activity**.
The project follows a production-oriented ML pipeline including data ingestion, validation, transformation, model training, prediction, logging, Dockerization, and cloud deployment preparation.

## 🚀 Project Overview

Phishing and malicious network activities are major cybersecurity threats. This project uses Machine Learning to analyze network security data and classify potentially malicious/phishing activity.

The project is structured using a modular ML pipeline rather than a single notebook, making it easier to maintain, test, deploy, and extend.

### 🔄 Workflow

```text
Raw Network Data
       ↓
Data Ingestion
       ↓
Data Validation
       ↓
Data Transformation
       ↓
Model Training
       ↓
Model Evaluation
       ↓
Model Artifact
       ↓
Prediction Pipeline
       ↓
Application / Deployment
```

## ✨ Key Features

* End-to-end Machine Learning pipeline
* Network security / phishing detection
* Data ingestion and validation
* Data transformation and preprocessing
* Model training and evaluation
* Separate training and prediction pipelines
* Model artifact management
* Logging and exception handling
* MongoDB integration
* Docker support
* AWS deployment configuration
* AWS ECR integration
* CI/CD workflow configuration
* Prediction output generation

## 🧰 Tech Stack

| Technology     | Purpose                   |
| -------------- | ------------------------- |
| Python         | Core programming language |
| Pandas         | Data processing           |
| NumPy          | Numerical computation     |
| Scikit-learn   | Machine Learning          |
| MongoDB        | Data storage              |
| PyMongo        | MongoDB connectivity      |
| Docker         | Containerization          |
| AWS            | Cloud deployment          |
| AWS ECR        | Docker image registry     |
| GitHub Actions | CI/CD                     |
| Flask          | Application/API layer     |

## 📁 Project Structure

```text
Network_Security_ML/
│
├── .github/
│   └── workflows/          # CI/CD workflows
│
├── Artifacts/              # Generated ML artifacts
│
├── Network_Data/           # Network security data
│
├── data_schema/            # Data schema and validation
│
├── final_model/            # Trained model artifacts
│
├── logs/                   # Application and pipeline logs
│
├── networksecurity/        # Main project package
│
├── prediction_output/      # Prediction results
│
├── templates/              # Application templates
│
├── valid_data/             # Validated data
│
├── app.py                  # Application entry point
├── main.py                 # ML pipeline entry point
├── push_data.py            # Data upload utility
├── test_mongodb.py         # MongoDB testing
│
├── Dockerfile              # Docker configuration
├── requirements.txt
```
