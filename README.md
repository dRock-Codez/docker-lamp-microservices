# 🐳 Docker LAMP Microservices Architecture

A robust, 3-tier web application stack built with **Docker Compose**. This project demonstrates **Infrastructure as Code (IaC)** principles by orchestrating Nginx, PHP-FPM, and MySQL containers into a seamless microservices network.

## 🏗️ Architecture
* **Web Server (Reverse Proxy):** Nginx (Port 8080)
* **Application Layer:** PHP 7.4-FPM
* **Database Layer:** MySQL 5.7 (Persistent Storage)
* **Orchestration:** Docker Compose

## 🚀 How to Run
1.  **Clone the repository:**
    ```bash
    git clone https://github.com/dRock-Codez/docker-lamp-microservices.git
    cd docker-lamp-microservices
    ```

2.  **Start the services:**
    ```bash
    docker compose up -d
    ```

3.  **View the application:**
    Open your browser and navigate to `http://localhost:8080`

4.  **Stop the services:**
    ```bash
    docker compose down
    ```

## 🛠️ Technical Highlights
* **Reverse Proxying:** Nginx handles HTTP traffic and forwards PHP requests to the FPM container via FastCGI.
* **Data Persistence:** MySQL data is mapped to a local volume, ensuring data survives container restarts.
* **Networking:** All containers communicate via a private Docker network.

---
*Built by [Uzoma](https://github.com/dRock-Codez)*
