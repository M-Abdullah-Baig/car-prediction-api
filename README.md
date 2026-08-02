# 🚗 Car Valuation Prediction API
A production-ready Machine Learning API built with FastAPI for vehicle valuation. The project includes a trained Random Forest model, an interactive Streamlit frontend, Docker support, and a REST API for real-time predictions.

## Project Overview:
This project predicts the estimated value of a vehicle based on its specifications using a machine learning model. The application exposes the model through a FastAPI REST API and also provides an interactive Streamlit interface for end users.

The project demonstrates an end-to-end machine learning workflow including:
Data preprocessing
Model training
Model serialization
REST API development
Input validation
Docker containerization
Frontend integration

## Features:
Vehicle valuation prediction
FastAPI REST API
Streamlit frontend
Pydantic request validation
Random Forest machine learning model
Dockerized application
Docker Hub deployment support
Clean project structure
Ready for cloud deployment (AWS EC2)

## Tech Stack:
### Machine Learning
Python
Scikit-learn
Pandas
NumPy

### Backend
FastAPI
Uvicorn
Pydantic

### Frontend
Streamlit

### DevOps
Docker
Docker Hub
Git
GitHub

## Project Structure:
car-prediction-api/
│
├── Dockerfile
├── .gitignore
├── .dockerignore
├── requirements.txt
├── runtime.txt
│
├── main.py
├── model.py
├── schema.py
├── train.py
├── streamlit_app.py
│
├── random_forest_model.pkl
├── feature_columns.pkl
├── cardekho_data.csv
│
└── README.md

## Machine Learning Workflow:
Dataset
    │
Data Preprocessing
    │
Feature Engineering
    │
Random Forest Model Training
    │
Save Model (.pkl)
    │
FastAPI
    │
REST API
    │
Docker
    │
Deployment

## API Endpoints
### Home
GET /
Returns a welcome message.

### Prediction
POST /predict
Predicts the estimated vehicle value.

## Interactive API Documentation
FastAPI automatically generates Swagger documentation.
http://localhost:8000/docs

## Installation
### Clone Repository
git clone https://github.com/M-Abdullah-Baig/car-prediction-fastapi

cd car-prediction-api

## Create Virtual Environment
Windows:
python -m venv .venv

### Activate
.venv\Scripts\activate

## Install Dependencies
pip install -r requirements.txt

## Run FastAPI
uvicorn main:app --reload

### Open
http://localhost:8000/docs

## Run Streamlit
streamlit run streamlit_app.py

## Docker
### Build Image
docker build -t <dockerhub-username>/car-prediction-api .

### Run Container
docker run -p 8000:8000 <dockerhub-username>/car-prediction-api

### Background mode:
docker run -d -p 8000:8000 abccode/car-prediction-api

### Push Image
docker push abccode/car-prediction-api

### Pull Image
docker pull abccode/car-prediction-api:latest

## AWS Deployment:
The project is designed for deployment on AWS EC2 using Docker.

Deployment workflow:

Docker Build
      │
Docker Hub
      │
AWS EC2
      │
Install Docker
      │
Pull Docker Image
      │
Run Container
      │
Access Public IP

## Development Workflow:
Develop
      │
Git
      │
GitHub
      │
Docker
      │
Docker Hub
      │
AWS EC2

## Future Improvements:
CI/CD using GitHub Actions
AWS ECR deployment
CloudWatch monitoring
Kubernetes deployment
Model versioning
Automated testing
Performance optimization
Authentication & authorization

## Learning Outcomes
This project demonstrates practical experience with:

Machine Learning model deployment
REST API development
FastAPI
Streamlit
Docker
Docker Hub
Git & GitHub
API testing
Cloud deployment workflow

## License
This project is intended for educational and portfolio purposes.

## Author
Muhammad Abdullah Baig
GitHub: https://github.com/M-Abdullah-Baig
