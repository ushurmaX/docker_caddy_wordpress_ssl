# WordPress + Caddy (Docker)
This project is a Docker-based setup for running WordPress with automatic HTTPS using Caddy.

## 🚀 Features

- WordPress (PHP-FPM)
- MariaDB database
- Caddy web server with automatic HTTPS (Let's Encrypt)
- Docker Compose setup
- Persistent storage using Docker volumes

## 🧱 Architecture

- Caddy handles HTTP/HTTPS and SSL certificates
- WordPress runs in PHP-FPM mode
- MariaDB stores application data
- Shared volume is used for WordPress files

## 📦 Services

- caddy
- wordpress
- db (MariaDB)

## ⚙️ Environment setup

Before running the project, create a `.env` file in the root directory:

```bash
MYSQL_DATABASE=wp_db
MYSQL_USER=wp_user
MYSQL_PASSWORD="your super secret password"
MYSQL_ROOT_PASSWORD="your super secret password"
```
## ⚙️ Usage

#### Start /  Stop /  Cleanup (⚠️ removes all data)

```bash
docker compose up -d
docker compose down
docker compose down -v
```

