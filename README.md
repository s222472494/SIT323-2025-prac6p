<<<<<<< HEAD
# SIT323-2025-prac6p
=======
# SIT323 - Practical 6.1P: Kubernetes Deployment

# Summary
This repo demonstrates deploying a Node.js microservice to a Kubernetes cluster.

# Features

- Containerised Node.js web application  
- Docker image pushed to Docker Hub  
- Kubernetes Deployment to manage pods  
- Kubernetes Service to expose the app  
- Can be run on Docker Desktop Kubernetes 

# Docker Image
Docker Hub: [s222472494/6.1p](https://hub.docker.com/r/s222472494/6.1p)
 
# Step-by-Step Setup Instructions

### Step 1: Clone the Repository

Start by cloning this repository to your local machine:

git clone https://github.com/s222472494/sit323-2025-prac6p.git
cd sit323-2025-prac6p


### Step 2: Build the Docker Image

docker login

docker build -t s222472494/6.1p:latest .

docker push s222472494/6.1p:latest

kubectl cluster-info

kubectl apply -f deployment.yaml

kubectl apply -f service.yaml

kubectl get pods

kubectl get services

http://localhost:3000




>>>>>>> 0c31197 (Initial commit with Dockerfile, Kubernetes configurations, and app)
