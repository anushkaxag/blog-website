
# About

A website built to explore and implement the concepts of microservices architecture! While the UI/UX is kept very basic, the primary focus was on learning and applying core principles of scalability, separation of concerns, and cross-service communication.

## Technologies Used:

*Backend:* Developed using **Node.js** and **Express.js** to ensure modular and scalable design.<br>
*Frontend:* Built with **React.js**, keeping it minimal to focus on functionality.<br>
*Deployment:* Each microservice is deployed in **Docker** containers and orchestrated by **Kubernetes** for seamless scalability.<br>
*Communication:* Enabled asynchronous *cross-service communication* via an *event bus*.<br>

## Tools and Workflow:

Used **Chocolatey** as the package manager for an efficient setup.<br>
Leveraged **Skaffold** for smooth development and deployment workflows.<br>

# Prerequisites:
Before running this project locally, make sure you have following installed:
- Node.js + Express.js + React.js
- Docker Desktop
- Kubernetes
- Kubectl
- Skaffold
- Ingress-Nginx

# To run:
- Clone the repository
- Install Dependencies: ```npm install```
- run: ```skaffold dev```

# To set up Docker + Kubernetes Cluster
- build Dockerimage - docker built -t {image name}
- push image on Docker hub - docker push {image name}
- For configuration (since we are using skaffold and ingress-nginx)
    - Deployment + service config file inside infra/k8s directory
    - Add config to skaffold.yaml file [Automation]
    - Configure Ingress-Nginx for routing requests from outside world


