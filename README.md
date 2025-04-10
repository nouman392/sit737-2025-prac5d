# Calculator Microservice – Task 5D  
**SIT737 – Cloud-Native Application Development**  
**Task 5D – Production Deployment to Google Cloud Container Registry (GCR)**

---

## Overview  
This project extends the Dockerized calculator microservice from Task 5.1P by publishing it to a private container registry on Google Cloud Platform (GCP). The image can now be securely pulled and executed from any environment, making it production-ready.

---

## Objectives  
- Containerize a Node.js microservice  
- Authenticate Docker with GCP  
- Tag and push the image to Google Container Registry (GCR)  
- Pull and run the image from GCR to validate production readiness

---

## Tools Used  
- [Node.js](https://nodejs.org/en/)  
- [Docker](https://www.docker.com/products/docker-desktop)  
- [Google Cloud SDK](https://cloud.google.com/sdk/docs/install)  
- [Git](https://git-scm.com)  
- [Visual Studio Code](https://code.visualstudio.com/)

---

Step 3: Build Docker Image
docker build -t calculator-microservice .
Step 4: Tag the Image for GCR
docker tag calculator-microservice gcr.io/sit737-25t1-ali-4ade49e/microservices-calculator
Step 5: Push Image to GCR
docker push gcr.io/sit737-25t1-ali-4ade49e/microservices-calculator
Step 6: Pull and Run Image from GCR
docker pull gcr.io/sit737-25t1-ali-4ade49e/microservices-calculator
docker run -p 3000:3000 gcr.io/sit737-25t1-ali-4ade49e/microservices-calculator
Open your browser:
http://localhost:3000/add?num1=5&num2=3
Expected response:
{ "result": 8 }

Benefits of Cloud Deployment
Portable – Pull and deploy anywhere

Cloud-native – Ready for Cloud Run, GKE, or CI/CD pipelines

Secure – Hosted in a private container registry
Reusable – Can serve as base for future microservices
