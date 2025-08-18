# 📝 Django Notes App

A full-stack **Notes Application** built with **Django, MySQL, Docker, and Nginx**.  
This project is containerized for easy deployment and demonstrates production-ready setup with reverse proxy and database integration.  

> ⚡ Inspired by [YouTube tutorial](link) but extended with Docker, Nginx, and server deployment.

---

## 🚀 Features
- User authentication (sign up, login, logout)
- Create, update, and delete notes
- Django + MySQL backend
- Dockerized deployment with `docker-compose`
- Nginx reverse proxy for production
- CI/CD ready (GitHub Actions workflow included)

---

## 🛠️ Tech Stack
- **Backend**: Django (Python 3.9)
- **Database**: MySQL
- **Web Server**: Nginx
- **Containerization**: Docker & Docker Compose
- **Deployment**: Ubuntu (AWS EC2)

---

## 📸 Screenshots

### Login Page
![Login Page](assets/screenshots/login.png)

### Notes Dashboard
![Dashboard](assets/screenshots/dashboard.png)

---

## ⚙️ Setup Instructions

### 1. Clone the repo
```bash
git clone https://github.com/YOUR-USERNAME/django-notes-app.git
cd django-notes-app
```

### 2. Build the app through the image
```bash
docker build -t notes-app .
```
### 3. Run the Containers
```bash
docker-compose up --build
```
