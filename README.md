🚗 React Tesla App

A modern Tesla UI built with React, Redux Toolkit, and TailwindCSS.
Containerized with Docker and deployed using Kubernetes.

🧩 Scripts
Command	Description
npm start	Run the app in development mode at http://localhost:3000

npm run build	Build the app for production (output in /build)
npm test	Run tests in watch mode
npm run eject	Eject CRA config (not reversible)


# 🚗 React Tesla App — Kubernetes Deployment

A simple **React Tesla clone** app containerized with **Docker** and deployed on **Kubernetes** (works with Minikube or AWS EKS).

---

## 🛠️ Technologies Used
- React + Redux Toolkit  
- Docker  
- Kubernetes (Deployment, Service, ConfigMap)  
- NGINX  

---

## ⚙️ Setup & Run Locally

### 1️⃣ Install dependencies
```bash
npm install

2️⃣ Start the app
bash
Copy code
npm start
Runs at http://localhost:3000

3️⃣ Build for production
bash
Copy code
npm run build

🐳 Docker Setup
Build and push image
bash
Copy code
docker build -t <your-dockerhub-username>/react-tesla-app:latest .
docker login
docker push <your-dockerhub-username>/react-tesla-app:latest

☸️ Deploy on Kubernetes
Apply manifests
bash
Copy code
kubectl apply -f configmap.yaml
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
Verify deployment
bash
Copy code
kubectl get pods
kubectl get svc
If using EKS → open LoadBalancer URL
If using Minikube → run:

bash
Copy code
minikube service react-tesla-service

📦 Files Included
css
Copy code
Dockerfile
deployment.yaml
service.yaml
configmap.yaml
public/
src/

✨ Author
Mos Richard
Deployed using Kubernetes and Docker 🚀
