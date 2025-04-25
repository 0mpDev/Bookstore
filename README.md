# Bookstore Management System

## 📚 Project Overview
A powerful and modern full-stack **Django-based Bookstore Management System**, built to handle inventory, user sessions, and custom admin workflows. Designed for real-world usage with authentication, cart management, and continuous deployment via Jenkins. Fully containerized using Docker for seamless development and deployment.

## 🚀 Key Features
- 🔐 Secure **User Registration/Login** using class-based views and manual HTML forms.
- 🛠️ **Custom Admin Dashboard** to add, update, or delete books — no default Django admin used.
- 📖 **Book Listings & Details** with intuitive UI.
- 🛒 **Add to Cart** feature powered by Django session framework.
- 🐳 Fully **Dockerized** using Docker & Docker Compose.
- 🔄 Integrated **Jenkins Pipeline** for CI/CD automation.

## 🧰 Tech Stack
- **Python 3.10**
- **Django 4.x**
- **PostgreSQL** (via Docker container)
- **Docker & Docker Compose**
- **Jenkins**
- **Gunicorn** as the WSGI server

## ⚙️ Getting Started

### 🔧 Prerequisites
- Docker & Docker Compose
- Jenkins (optional, for CI/CD)

### ▶️ Run the App with Docker
1. **Start the Docker containers**:
   
   ```
   docker-compose up --build
   ```
2. **Apply migrations**:
   ```
   docker-compose run web python manage.py migrate
   ```
3. **Create a superuser (optional for admin access)**:
   ```
   docker-compose run web python manage.py createsuperuser
   ```
4. **Access the app at `http://localhost:8000`**

### 🔁 Jenkins CI/CD Pipeline
The `Jenkinsfile` automates the following:
- Builds the Docker image
- Executes Django tests
- Deploys the app using Docker Compose

## 📸 Screenshots
![WhatsApp Image 2025-04-25 at 20 36 16_50fb2aa7](https://github.com/user-attachments/assets/2bd797c5-c203-4cfc-89b9-f0ebc92a67bb)  
![WhatsApp Image 2025-04-25 at 20 39 50_d56aae41](https://github.com/user-attachments/assets/e2ed30e2-77c1-4b5a-ab05-b1ca4be8a2f3)  
![WhatsApp Image 2025-04-25 at 20 46 44_fcd374b6](https://github.com/user-attachments/assets/99a75902-426e-4e1c-afed-67ed1f6b14f2)  
![WhatsApp Image 2025-04-25 at 20 55 27_14c800b3](https://github.com/user-attachments/assets/1a6f4064-deaa-498f-bb64-cf71e0dfff8e)

## 📝 Notes
- Forms are custom-built in plain HTML without using Django Forms.
- Shopping cart is managed through server-side sessions.
- A completely **custom admin interface** — Django admin is not used.

