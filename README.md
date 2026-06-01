# Employee-Management-System-Dockerized-LEMP-Stack-

A lightweight, full-stack web application designed for HR departments to manage employee directories and relational department assignments. The entire application infrastructure is isolated and orchestrated using **Docker** and **Docker Compose**, running a classic **LEMP stack** (Linux, Nginx, MySQL, PHP) inside an Ubuntu environment.

## 🚀 Features
* **Full CRUD Operations:** Support for adding new employee records, reading/displaying real-time database inputs, and securely executing deletions.
* **Relational Database Design:** Configured a secure one-to-many relationship using SQL foreign keys mapping employees to specific corporate departments.
* **Security-First Approach:** Implemented PHP PDO/MySQLi Prepared Statements to mitigate SQL injection vulnerabilities.
* **Data Persistence:** Utilized named Docker Volumes to guarantee database states persist safely across container restarts or teardowns.
* **Modern UI:** Styled using responsive Bootstrap 5 elements for a clean dashboard view.

---

## 🛠️ Tech Stack & Architecture
* **Frontend/Backend:** PHP 8.x, HTML5, Bootstrap 5
* **Web Server:** Nginx (configured as a reverse proxy for PHP-FPM)
* **Database:** MySQL 8.0 
* **DevOps/Infrastructure:** Docker, Docker Compose, VirtualBox (Ubuntu Server Host)

---

## 📁 Project Structure
```text
my-php-app/
├── docker-compose.yml       # Docker infrastructure blueprint
├── README.md                # Project documentation
└── src/                     # Application source code
    ├── index.php            # Main HR Dashboard UI & employee view
    ├── add_employee.php     # Backend processing script for new hires
    ├── delete_employee.php  # Secure entry deletion execution
    └── includes/
        └── db.php           # Centralized MySQL database connection module
