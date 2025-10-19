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

