# 🚀 Docker Multiple PHP Environment

Satu container Docker, banyak versi PHP. Proyek ini memudahkan Anda menjalankan PHP versi 5.6, 7.4, dan 8.2 secara bersamaan menggunakan Nginx dan Docker Compose, lengkap dengan phpMyAdmin!

---

## 📦 Requirement

- ✅ Docker `28.1.1`, build `4eba377`  
- ✅ Docker Compose (sudah terintegrasi di Docker Desktop 28+)

---

## 🔧 Fitur

- 🐘 PHP 5.6 – akses di: [`http://localhost.php5`](http://localhost.php5)  
- 🐘 PHP 7.4 – akses di: [`http://localhost.php7`](http://localhost.php7)  
- 🐘 PHP 8.2 – akses di: [`http://localhost`](http://localhost)  
- 🛠️ phpMyAdmin – akses di: [`http://localhost.db`](http://localhost.db)  
- 🌐 Nginx sebagai reverse proxy  
- 💾 Volume persistence untuk database MySQL  

---

## 🔧 Config

- GANTI_PASSWORD_ANDA   : ganti password anda

---

## 📁 Struktur Folder

```bash
docker_multiple_php/
├── docker-compose.yml
├── nginx/
│   └── default.conf
├── localhost/         # Untuk PHP 8.2
│   └── index.php
├── localhost7/        # Untuk PHP 7.4
│   └── index.php
├── localhost5/        # Untuk PHP 5.6
│   └── index.php
└── mysql_data/        # Data MySQL
