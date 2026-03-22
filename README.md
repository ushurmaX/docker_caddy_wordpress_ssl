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
