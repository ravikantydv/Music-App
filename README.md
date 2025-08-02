# 🎵 MyMusicApp - A Django-Based Music Management System

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Python](https://img.shields.io/badge/python-3.10+-blue.svg)
![Dockerized](https://img.shields.io/badge/docker-ready-success)
![Status](https://img.shields.io/badge/status-active-brightgreen)

Welcome to **MyMusicApp**, a modern web application to manage, stream, and organize music using Django. It is fully containerized with **Docker** and uses **SQLite** as its default database for quick setup.

---

## 🚀 Features

- 🎧 Upload and manage music files
- 📂 Categorize tracks by genre, artist, and album
- 🕵️ User authentication and admin panel
- 🐳 Docker and Docker Compose support
- 🔐 Environment variable management via `.env`
- 🎛 Built with scalability and security in mind

---

## 🛠️ Project Structure

├── .env # Environment variables (Not tracked)
├── Dockerfile # Docker image instructions
├── docker-compose.yaml # Docker Compose configuration
├── db.sqlite3 # SQLite database file
├── manage.py # Django project entry point
├── music/ # Django app: music management
├── mymusicapp/ # Django project settings
├── requirements.txt # Python dependencies
└── README.md # You are here!

## 🔧 Installation

### ✅ Prerequisites
- Python 3.10+
- Docker & Docker Compose

---

### 💻 Local Development Setup

```bash
# Clone the repository
git clone https://github.com/yourusername/mymusicapp.git
cd mymusicapp

# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run migrations
python manage.py migrate

# Start the development server
python manage.py runserver


# Build and start containers
docker-compose up --build

# Access the app at http://localhost:8000/


DEBUG=True
SECRET_KEY=your_secret_key_here
ALLOWED_HOSTS=localhost,127.0.0.1
