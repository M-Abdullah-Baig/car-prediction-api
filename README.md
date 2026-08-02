# 🚗 Car Valuation Prediction API
A production-ready Machine Learning API built with FastAPI for vehicle valuation. The project includes a trained Random Forest model, an interactive Streamlit frontend, Docker support, and a REST API for real-time predictions.

## Project Overview:
This project predicts the estimated value of a vehicle based on its specifications using a machine learning model. The application exposes the model through a FastAPI REST API and also provides an interactive Streamlit interface for end users.

The project demonstrates an end-to-end machine learning workflow including:

- Data preprocessing

- Model training

- Model serialization

- REST API development

- Input validation

- Docker containerization

- Frontend integration

## Features:

- Vehicle valuation prediction

- FastAPI REST API

- Streamlit frontend

- Pydantic request validation

- Random Forest machine learning model

- Dockerized application

- Docker Hub deployment support

- Clean project structure

- Ready for cloud deployment (AWS EC2)

## Tech Stack:
### Machine Learning

- Python

- Scikit-learn

- Pandas

- NumPy

### Backend

- FastAPI

- Uvicorn

- Pydantic

### Frontend

- Streamlit

### DevOps

- Docker

- Docker Hub

- Git

- GitHub

## 📁 Project Structure

```text
car-prediction-fastapi/
│
├── Dockerfile                 # Docker configuration
├── .dockerignore              # Files ignored during Docker build
├── .gitignore                 # Files ignored by Git
├── README.md                  # Project documentation
├── requirements.txt           # Python dependencies
├── runtime.txt                # Runtime configuration
│
├── main.py                    # FastAPI application
├── model.py                   # Prediction logic
├── schema.py                  # Pydantic request/response models
├── train.py                   # Model training script
├── streamlit_app.py           # Streamlit frontend
│
├── random_forest_model.pkl    # Trained ML model
├── feature_columns.pkl        # Feature metadata
├── cardekho_data.csv          # Dataset
```

## Machine Learning Workflow:
Dataset

  → Data Preprocessing
  
  → Feature Engineering
  
  → Model Training (Random Forest)
  
  → Save Model (.pkl)
  
  → FastAPI
  
  → REST API
  
  → Docker
  
  → Deployment

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

cd car-prediction-fastapi

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
docker build -t abccode/car-prediction-fastapi .

### Run Container
docker run -p 8000:8000 abccode/car-prediction-fastapi

### Background mode:
docker run -d -p 8000:8000 abccode/car-prediction-fastapi

### Push Image
docker push abccode/car-prediction-fastapi

### Pull Image
docker pull abccode/car-prediction-fastapi:latest

## AWS Deployment:
The project is designed for deployment on AWS EC2 using Docker.

### Deployment workflow:
Docker Build

→ Push to Docker Hub

→ Create AWS EC2 Instance

→ Install Docker

→ Pull Docker Image

→ Run Docker Container

→ Configure Security Group

→ Access API via Public IP

## Development Workflow:
Develop Code

→ Git

→ GitHub

→ Dockerize Application

→ Push Image to Docker Hub

→ Deploy on AWS EC2

## Future Improvements:

- Implement CI/CD using GitHub Actions
  
- Deploy the application on AWS EC2
  
- Add model performance monitoring and logging
  
- Implement automated testing
  
- Add authentication and authorization

## Learning Outcomes
This project demonstrates practical experience with:

- Data preprocessing
  
- Feature engineering

- Machine Learning model training
  
- Model serialization using Pickle (.pkl)
  
- REST API development using FastAPI
  
- Request validation with Pydantic
  
- Frontend development using Streamlit
  
- Docker containerization
  
- Git and GitHub version control
  
- API testing using Swagger UI
  
- Cloud deployment workflow (AWS EC2)

## License
This project is intended for learning, portfolio, and demonstration purposes. It showcases practical skills in Machine Learning, FastAPI, Docker, and API development.

## Author
Muhammad Abdullah Baig

GitHub: https://github.com/M-Abdullah-Baig
