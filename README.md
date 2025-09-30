🚀 WSThreeTierAppChallenge (Simplified Version)

Maintained by Iftikhar Hussain

This is a simplified version of the classic Three-Tier Web Application, built with ReactJS and NodeJS. The focus here is on making the frontend and backend work together locally, while laying the groundwork for Kubernetes deployment and database integration in the future.

📌 What’s This About

Originally, the app had a full MongoDB backend, but for now I’ve removed it to make local testing easier. So, what’s in this repo:

Frontend: ReactJS

Backend: NodeJS + Express

The database will come back later, and when it does, it’ll run on Kubernetes so we can simulate a real production setup.

🏗️ Architecture (High-Level)
<img width="1024" height="578" alt="image" src="https://github.com/user-attachments/assets/6eac063f-096a-47da-81e6-809d8103f1e6" />


Frontend (ReactJS) → The user interface.

Backend (NodeJS + Express) → Handles API requests and business logic.

Database (MongoDB) → Coming soon via Kubernetes.
[
(If you have a diagram, you can insert it here.)](https://www.percona.com/blog/wp-content/uploads/2021/10/blog-mongo-migrate-1024x582.png)

🚀 Running It Locally

Step 1: Clone the Repo
git clone https://github.com/iftikhar69/WSThreeTierAppChallenge-Public.git
cd WSThreeTierAppChallenge-Public

Step 2: Start the Backend
cd backend
npm install
npm start

Step 3: Start the Frontend
cd frontend
npm install
npm start

Runs on → http://localhost:3000

Step 4: Open the App

Go to http://localhost:3000 in your browser.

The frontend talks to the backend at port 8080.

☸️ Kubernetes (What’s Ready / Next)

I’ve already prepared Kubernetes manifests for the full three-tier setup:

namespace.yaml → Create a separate namespace.

mongodb.yaml → MongoDB deployment + service.

backend.yaml → Backend deployment + service.

frontend.yaml → Frontend deployment + service.

Quick Deployment Steps:
kubectl apply -f k8s-manifests/namespace.yaml
kubectl apply -f k8s-manifests/mongodb.yaml
kubectl apply -f k8s-manifests/backend.yaml
kubectl apply -f k8s-manifests/frontend.yaml
kubectl get pods -n twstier
kubectl get svc -n twstier

Notes:

Docker images must be built locally or pushed to a registry like DockerHub / ECR.

MongoDB is currently a local free deployment.

✅ What’s Done

Frontend and backend running locally.

Kubernetes manifests for backend, frontend, and MongoDB are ready.

Everything pushed to GitHub for easy cloning and deployment.

Deployment plan is ready for Kubernetes and AWS EKS.

🔜 Next Steps

Connect MongoDB with backend in Kubernetes.

Deploy the full app on local Kubernetes or AWS EKS.

Automate deployments with CI/CD (Jenkins / ArgoCD).

Optionally add monitoring (Prometheus / Grafana).

🛠️ Tech Stack
| Layer      | Technology                     |
| ---------- | ------------------------------ |
| Frontend   | ReactJS ⚛️                     |
| Backend    | NodeJS + Express 🚀            |
| Database   | MongoDB ❌ (to be added)        |
| Deployment | Kubernetes / AWS EKS           |
| CI/CD      | Jenkins / ArgoCD (planned)     |
| Monitoring | Prometheus / Grafana (planned) |

👨‍💻 About Me

I’m Iftikhar Hussain, learning backend and cloud engineering while exploring AI/ML.
My goal is to build scalable applications and become a successful software engineer & entrepreneur.
