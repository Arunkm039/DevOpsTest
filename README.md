# 🔧 GitHub Gist API Service

A simple HTTP API built with Flask that fetches a user's public GitHub Gists. The service includes automated tests, pagination, optional caching, and Docker support.

---

## 🚀 Features

- `GET /<username>` returns public Gists for a GitHub user.
- Supports pagination: `?page=<num>&per_page=<num>`
- In-memory caching using `lru_cache`
- Automated testing using `pytest`
- Dockerized setup for easy deployment

---

## 🗂️ Project Structure
.
├── app.py # Flask API server
├── test_app_pytest.py # API test suite using pytest
├── Dockerfile # Docker configuration
├── requirements.txt # Python dependencies (optional)
└── README.md # You're here!


---

## 🧰 Prerequisites

- Python 3.8+
- `pip` (Python package manager)
- Docker (for containerized usage, optional)

---

## 🧪 Running Locally

### 1. Clone the repository

```bash
git clone <your-repo-url>
cd <your-repo-folder>
