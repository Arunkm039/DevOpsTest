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

## 📁 Project Structure

The repository contains a minimal Flask-based API with Docker support and automated tests:

```text
github-gist-api/
│
├── app.py               # Flask web server
├── test_app.py          # Automated test cases
├── requirements.txt     # Python dependencies
├── Dockerfile           # Docker image for API and tests
└── docker-compose.yml   # Docker Compose orchestration

```

---

## ⚙️ Prerequisites

Ensure the following are installed:

- [Docker](https://www.docker.com/get-started)
- [Docker Compose](https://docs.docker.com/compose/install/) (if not included with Docker)

---

## Quick Start

### Step 1: Clone the Repo

```bash
git clone https://your-repo-url/github-gist-api.git
cd github-gist-api
```

### Step 2: Build and Start Services
**docker-compose up --build**

This will:

* Build the Docker image from Dockerfile

* Start the Flask API (web) on http://localhost:8080

* Run the automated test cases (test_runner) once and print results in logs

* Keep the Flask API running regardless of test outcome

## API Usage

Once running, try:

curl http://localhost:8080/octocat

You can also specify pagination:
curl "http://localhost:8080/octocat?page=2&per_page=5"

## How It Works

* Dockerfile builds a Python 3.10 image with Flask and requests installed.

* web service runs app.py and exposes port 8080

* test_runner waits for web to start, then runs test_app.py using real HTTP requests to http://web:8080

* Docker Compose handles inter-container networking (web is used as the hostname inside test_runner)




