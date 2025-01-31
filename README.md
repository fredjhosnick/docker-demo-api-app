# 🚀 Dockerized Django API App

This project is a **Django REST API**, fully containerized using **Docker** and **Docker Compose** for seamless development and deployment.

## 📌 Technologies Used
- 🐍 **Python 3.7**
- 🏗 **Django 3.2**
- 🌐 **Django REST Framework**
- 🐳 **Docker & Docker Compose**
- 💾 **SQLite** (default) or **PostgreSQL** (optional)

## 📖 Prerequisites
Before running the project, ensure you have the following installed:
- [Docker](https://www.docker.com/get-started)
- [Docker Compose](https://docs.docker.com/compose/install/)
- Git

---

## 🚀 Getting Started

###1️⃣ Clone the Repository
Open a terminal and run:
```sh
git clone https://github.com/fredjhosnick/docker-demo-api-app.git
cd docker-demo-api-app

###2️⃣ Build and Run the Containers
docker-compose up --build -d

###3️⃣ Apply Database Migrations
Once the containers are running, apply Django migrations:
docker-compose exec app python manage.py migrate

###4️⃣ Create a Superuser (Optional)
If you want to access the Django Admin panel:
docker-compose exec app python manage.py createsuperuser

###5️⃣ Access the API

Open in your browser: http://localhost:8080
Django Admin Panel: http://localhost:8080/admin


docker-demo-api-app/
│── app/                 # Django project files
│── Dockerfile           # Docker image configuration
│── docker-compose.yml   # Docker services definition
│── requirements.txt     # Python dependencies
│── README.md            # Project documentation

###6Deployment (Optional)
To deploy the app to a cloud platform, consider:

Render
Railway
Fly.io
Heroku (with Docker support)

