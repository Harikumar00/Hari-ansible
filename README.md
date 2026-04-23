MERN DevOps Project (Travel Memory)

## 📌 Overview

This project demonstrates end-to-end deployment of a MERN (MongoDB, Express, React, Node.js) application using DevOps tools on AWS.

The application allows users to add and view travel experiences.

---

## 🏗️ Architecture

User → EC2 (Web Server: Frontend + Backend) → EC2 (Database Server: MongoDB - Private IP)

* Frontend: React (served on port 3000)
* Backend: Node.js + Express (port 3001)
* Database: MongoDB (private EC2 instance)
* Infrastructure: Terraform
* Configuration: Ansible
* Process Manager: PM2

---

## ⚙️ Tech Stack

* **Frontend:** React.js
* **Backend:** Node.js, Express.js
* **Database:** MongoDB
* **DevOps Tools:** Terraform, Ansible
* **Cloud:** AWS EC2
* **Process Manager:** PM2

---

## 🚀 Features

* Add travel experiences
* View all trips
* Featured trips section
* REST API integration

---

## 🔗 API Endpoints

| Method | Endpoint  | Description    |
| ------ | --------- | -------------- |
| GET    | /trip     | Get all trips  |
| GET    | /trip/:id | Get trip by ID |
| POST   | /trip     | Add new trip   |

---

## 🛠️ Setup Instructions

### 🔹 Backend Setup

```bash
cd backend
npm install
npm start
```

### 🔹 Frontend Setup

```bash
cd frontend
npm install
npm run build
```

---

## ☁️ Deployment

### 🔹 Terraform

* Used to provision EC2 instances
* Created separate instances for:

  * Web server
  * Database server

### 🔹 Ansible

* Installed dependencies (Node.js, Git)
* Cloned repository
* Installed packages
* Built frontend
* Started backend using PM2

---

## 🌐 Live Application

Frontend: http://13.57.13.74:3000
Backend: http://13.57.13.74:3001

---

## 🔐 Security Considerations

* MongoDB runs on a private IP
* Sensitive files excluded using `.gitignore`:

  * `.env`
  * `.pem`
  * `node_modules`
  * Terraform state files

---

## 📚 Key Learnings

* End-to-end deployment of MERN stack
* Infrastructure automation using Terraform
* Configuration management with Ansible
* Debugging real-world deployment issues
* Handling networking and security in AWS

---
## Screenshots

Web Ec2 instance
<img width="1440" height="900" alt="Screenshot 2026-04-23 at 11 54 53" src="https://github.com/user-attachments/assets/3673db1d-e9b1-4089-8e82-df7a15a40ce7" />

DB Ec2 instance
<img width="1440" height="900" alt="Screenshot 2026-04-23 at 11 55 51" src="https://github.com/user-attachments/assets/50edb57b-1889-4e72-afac-1db85e71a29e" />








## 👨‍💻 Author

**Hari Kumar**
