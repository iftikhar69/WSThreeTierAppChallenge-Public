# WSThreeTierAppChallenge (Modified by Iftikhar)

## Overview  

This repository contains a simplified version of the **WSThreeTierAppChallenge**.  
Originally, it was a full **Three-Tier Web Application** (Frontend + Backend + Database), but in this repo I (Iftikhar) have kept only the **Frontend** and **Backend**.  

I plan to connect the backend with a database (MongoDB) later, possibly via **Kubernetes** manually.  

---

## Project Structure  

📦 WSThreeTierAppChallenge
┣ 📂 frontend → ReactJS frontend code
┣ 📂 backend → NodeJS/Express backend code
┗ 📜 README.md → Project documentation


---

## Tech Stack  

- **Frontend**: ReactJS  
- **Backend**: NodeJS + Express  
- **Database**: (Removed for now, will be connected later manually)  

---

## Getting Started  

### 1. Clone the Repository  

```bash
git clone https://github.com/iftikhar69/WSThreeTierAppChallenge-Public.git
cd WSThreeTierAppChallenge-Public

2. Run the Backend

cd backend
npm install
npm start

The backend should start on http://localhost:5000

(or the port you configure).
3. Run the Frontend

cd frontend
npm install
npm start

The frontend should start on http://localhost:3000

.
Future Plan

    Add MongoDB integration

    Deploy with Kubernetes (EKS)

    Setup CI/CD pipeline

Author

👨‍💻 Iftikhar
Learning backend & cloud technologies, aiming to become a skilled software engineer and build scalable apps 🚀
Contribution

Right now, this repo is simplified for my personal learning. Contributions are welcome — feel free to fork and make improvements!


---

👉 Next Step: Do you also want me to **generate placeholder `README.md` files for `/frontend` and `/backend`** folders (explaining how to run each)? That way, anyone opening the repo immediately understands how to use each part.

