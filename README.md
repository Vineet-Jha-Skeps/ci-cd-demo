# 🐍 CI/CD Demo App

A simple **Hello World** Python web application containerized with **Docker** and automated deployment using **GitHub Actions CI/CD**.

---

### 🚀 Features

* Minimal Python web app using Flask
* Docker-ready containerization
* Fully automated CI/CD pipeline using GitHub Actions
* Unit testing as part of the workflow

---

### 📂 Project Structure

```
ci-cd-demo/
├── app.py              # Flask app returning Hello World
├── test.py             # Basic automated test
├── requirements.txt    # Python dependencies
├── Dockerfile          # Build instructions for container image
└── .github/workflows/  # GitHub Actions CI/CD config
```

---

### ⚙️ CI/CD Pipeline Overview

GitHub Actions workflow automates:

| Stage                | Purpose                                      |
| -------------------- | -------------------------------------------- |
| Checkout             | Pull latest code                             |
| Install dependencies | Set up Python environment                    |
| Test                 | Run basic unit tests                         |
| Docker Build         | Build container image with version tags      |
| Docker Push          | Push image to DockerHub (using repo secrets) |

Required Secrets:

* `DOCKERHUB_USERNAME`
* `DOCKERHUB_TOKEN`
* `REPO_NAME`

---

### 🧪 Running Tests Locally

```sh
python3 -m pip install -r requirements.txt
pytest -v
```

---

### 👨‍💻 Author

**Vineet Jha**
Demo project showcasing CI/CD automation skills with Docker & GitHub Actions.
