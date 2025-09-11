# PetsEHR Demo

**PetsEHR** is a lightweight **Electronic Health Records (EHR) system for veterinary clinics**.  
This repository provides a demo edition that allows you to explore the platform, run it locally, and experiment with its features.

> ⚠️ Note: This edition is intended as a **demo preview** of PetsEHR. Certain features such as advanced role management, billing, and production infrastructure are not included.

---

## 🐾 What You Can Do with the Demo
- Register pets and record visit history.  
- Manage basic owner and clinic information.  
- Explore REST and GraphQL APIs for integration.  
- Run the system locally with Docker for easy evaluation.  

---

## 🛠️ Tech Stack
- **Backend**: FastAPI (Python) with REST + GraphQL  
- **Frontend**: Vue 3 + TypeScript + Tailwind CSS  
- **Database**: PostgreSQL (Dockerized)  
- **Messaging**: Redis Streams (demo pub/sub flow)  
- **Authentication**: OAuth2 + JWT (basic demo implementation)  
- **Infrastructure**: Docker Compose (local dev), GitHub Actions (CI/CD)  

---

## 🚀 Getting Started
```bash
# Clone repo
git clone https://github.com/YOUR-ORG/pets-ehr-demo.git
cd pets-ehr-demo

# Start local environment
docker-compose up --build

