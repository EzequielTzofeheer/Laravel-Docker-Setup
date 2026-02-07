# Laravel Docker Setup

![Laravel](https://img.shields.io/badge/Laravel-12.x-red)
![PHP](https://img.shields.io/badge/PHP-8.3%2B-blue)
![Docker](https://img.shields.io/badge/Docker-Ready-blue)
![License](https://img.shields.io/badge/License-MIT-green)

A reusable and standardized **Docker-based development environment** for **Laravel 12**, designed to accelerate project setup and ensure consistency across applications.

---

## 📌 What is this?

**Laravel Docker Setup** is a base repository that provides a complete local development environment for Laravel 12 using Docker and Docker Compose.

It delivers a ready-to-use infrastructure with all essential services preconfigured, allowing developers to focus on building features instead of setting up environments.

---

## 🎯 What is it for?

This project is intended to be used as a **starting point** for new Laravel applications that require:

- A fully configured Docker environment
- Consistent setup across multiple projects
- Faster onboarding for new developers
- Reduced time spent on infrastructure configuration

Ideal for teams and solo developers who want a **clean, predictable and reproducible** Laravel environment.

---

## 🧠 How does it work?

The project uses **Docker Compose** to orchestrate multiple containers, each with a specific responsibility:

- **App**: PHP container where the Laravel application runs
- **Queue**: Dedicated worker container for processing Laravel queues
- **Nginx**: Web server responsible for handling HTTP requests
- **MySQL**: Relational database
- **Redis**: Cache and queue backend
- **PHPMyAdmin**: Web interface for database management

All services communicate through a dedicated Docker bridge network.

---

## 🚀 Quick Installation

### 1️⃣ Clone the repository

```bash
git clone https://github.com/EzequielTzofeheer/Laravel-Docker-Setup
```

2️⃣ Access the project directory

```bash
cd Laravel-Docker-Setup
```

3️⃣ Create the environment file

```bash
cp .env.example .env
```

4️⃣ Build and start the containers

```bash
sudo docker compose up -d
```

5️⃣ Access the Docker container

```bash
sudo docker compose exec app bash
```

6️⃣ Install Laravel dependencies

```bash
composer install
```

7️⃣ Generate the application key

```bash
php artisan key:generate
```

---

## 🎯 Goal / Purpose

The main goals of this repository are:

- Provide a standardized Laravel Docker setup
- Serve as a reusable foundation for multiple projects
- Improve development speed and consistency
- Act as a versioned, stable base using tags instead of branches

This repository is not a final product, but a solid foundation to build upon.

---

## 🧱 Tech Stack

- PHP 8.3+
  - Laravel 12.x
- Docker
  - Docker Compose
- Nginx
- MySQL 8
- PHPMyAdmin
- Redis

---

## 🧩 Compatibility

- PHP: 8.3 or higher
- Laravel: 12.x
- Docker: 24 or higher
- Docker Compose: 2 or higher
- Supported OS:
  - Linux
  - macOS
  - Windows (WSL2)

---

## 🤝 Contributing

Contributions are welcome.

You can contribute by:

- Opening Issues
- Submitting Pull Requests
- Suggesting improvements to the setup or documentation

Please ensure that changes remain generic and reusable.

---

## 🙌 Credits

- Laravel Framework
- Docker
- Open Source Community

---

## ⭐ Support

If this repository was useful to you, consider leaving a ⭐ on GitHub.

It helps support the project and encourages continuous improvement.

---

## 👤 Author

Developed and maintained by **Ezequiel Tzofeheer**

**Full Stack Developer** with a strong focus on building clean, scalable and secure applications.

**Core areas of interest:**

- Clear and maintainable architecture
- High productivity and developer experience
- Cyber security and data protection
- Software engineering best practices
- Performance and cost efficiency

---

📄 License

This project is licensed under the MIT License.

See the LICENSE file for more details.
