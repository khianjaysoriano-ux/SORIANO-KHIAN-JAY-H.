# Two-Tier Architecture

## 1. The Web/Application Tier

The web/application tier uses Nextcloud to provide the user interface for the private cloud storage system. It handles HTTP requests from users and allows them to access and manage their files through a web browser.

## 2. The Database Tier

The database tier uses MariaDB to store persistent information required by Nextcloud, such as user accounts, file metadata, and application settings.

## 3. Why Separate Them?

Separating the web application and database into different containers makes the system easier to manage, maintain, and troubleshoot. Each container has a specific responsibility and can be updated or scaled independently when needed. Container separation also helps organize services, although additional security measures are still required to protect the application and database.

## 4. Architecture Used

- **Application:** Nextcloud
- **Database:** MariaDB 10.6
- **Deployment tool:** Docker Compose
- **Access port:** 8080
- **Database hostname:** database
