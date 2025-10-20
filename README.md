# GitHub Gist API - Dockerized Flask App with Automated Tests

This project provides a Dockerized Flask-based API that fetches public gists from GitHub for a given user. It includes automated tests that validate the live API using Docker Compose.

---

## 📦 Features

- Flask API server exposed on **port 8080**
- Endpoint: `GET /<username>?page=<int>&per_page=<int>`
- Real-time testing of the live server via HTTP
- Full setup using Docker and Docker Compose
- Server continues running even if tests fail

---

## 🗂️ Project Structure

gist-api/
│
├── app.py # Flask web server
├── test_app.py # Automated test cases
├── requirements.txt # Python dependencies
├── Dockerfile # Shared image for API and tests
└── docker-compose.yml # Orchestration of services
