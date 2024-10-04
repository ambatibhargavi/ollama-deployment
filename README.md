# ollama-deployment
# Custom LLM using Ollama

This project demonstrates the creation and deployment of a custom Large Language Model (LLM) using **Ollama**, trained on a user-provided CSV file. The model functions as a Q&A system, allowing users to interact with the data seamlessly.

## Features

- **Custom Data**: Trained on a specific CSV file, allowing for tailored responses to user queries.
- **Interactive Q&A**: Provides an intuitive interface for querying the data.
- **Dockerized Deployment**: Ensures a consistent environment through Docker.
- **Kubernetes Orchestration**: Manages the deployment for scalability and reliability.

## Project Structure

Custom-LLM-Ollama/ ├── README.md ├── Dockerfile ├── requirements.txt ├── model/ │ ├── train.py │ ├── utils.py │ ├── config.json │ └── your_data.csv ├── deployment/ │ ├── kubernetes/ │ │ ├── deployment.yaml │ │ └── service.yaml │ └── docker-compose.yaml └── docs/ ├── flowchart.png └── project_overview.md

## Install dependencies:

pip install -r requirements.txt

## Build the Docker image:

docker build -t custom-llm .

## Deploy to Kubernetes:

kubectl apply -f deployment/kubernetes/deployment.yaml
kubectl apply -f deployment/kubernetes/service.yaml

![DALL·E 2024-10-04 14 44 48 - A detailed flowchart illustrating the deployment process of an Ollama model using Python, Docker, and Kubernetes  The flowchart should have a clear, s](https://github.com/user-attachments/assets/ba56f62d-a5aa-4500-9ba2-3e86a07f883f)
<img width="1440" alt="Screenshot 2024-10-04 at 14 11 22" src="https://github.com/user-attachments/assets/ed7b06ec-9ea7-416c-bb92-377c1d6b99bc">
