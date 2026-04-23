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

Web Ec2 instance:
<img width="1440" height="900" alt="Screenshot 2026-04-23 at 11 54 53" src="https://github.com/user-attachments/assets/3673db1d-e9b1-4089-8e82-df7a15a40ce7" />

DB Ec2 instance:
<img width="1440" height="900" alt="Screenshot 2026-04-23 at 11 55 51" src="https://github.com/user-attachments/assets/50edb57b-1889-4e72-afac-1db85e71a29e" />

Website Curl Terminal:
<img width="1440" height="900" alt="Screenshot 2026-04-23 at 11 29 54" src="https://github.com/user-attachments/assets/2cb187a2-2522-4d37-8b35-cd431012ca0b" />

<img width="1440" height="900" alt="Screenshot 2026-04-23 at 11 30 00" src="https://github.com/user-attachments/assets/5ca20f5b-f01f-49e2-969c-500282d567b6" />

Website homepage in browser:
<img width="1440" height="900" alt="Screenshot 2026-04-23 at 11 28 43" src="https://github.com/user-attachments/assets/68c5939b-7b2b-477b-ae5e-87968ffbab82" />

Website Add experience page in browser:
<img width="1440" height="900" alt="Screenshot 2026-04-23 at 11 28 55" src="https://github.com/user-attachments/assets/f4c416ec-a165-4ecd-9aba-acef505ffe2a" />

Website trip details page in browser:
<img width="1440" height="900" alt="Screenshot 2026-04-23 at 11 29 13" src="https://github.com/user-attachments/assets/14a6647c-9216-4680-a4ad-425d907da1d6" />

Terraform Apply:
<img width="1440" height="900" alt="Screenshot 2026-04-23 at 12 21 59" src="https://github.com/user-attachments/assets/e53b5845-1e1b-451b-9f5f-db5695cd3915" />

Ansible inventory.ini :
<img width="1440" height="900" alt="Screenshot 2026-04-23 at 12 25 09" src="https://github.com/user-attachments/assets/7c145483-b89b-4f8a-a8f2-b3cf682ae3bc" />

Ansible web.yml : 
<img width="1440" height="900" alt="Screenshot 2026-04-23 at 12 26 01" src="https://github.com/user-attachments/assets/0588eee3-2b6a-42c4-b629-e179c64b094e" />

PM2 Status : 
<img width="1440" height="900" alt="Screenshot 2026-04-23 at 12 27 06" src="https://github.com/user-attachments/assets/451835c8-880c-4c54-ba5f-97c7ea0b0599" />

Mongo Db Running :
<img width="1440" height="900" alt="Screenshot 2026-04-23 at 12 30 37" src="https://github.com/user-attachments/assets/fb7bb45e-166c-451f-afad-0011d010cef4" />

PM2 logs BE : 
<img width="1440" height="900" alt="Screenshot 2026-04-23 at 12 35 39" src="https://github.com/user-attachments/assets/6304faec-8103-4af3-8bc4-d1b088fe0e7d" />




## 👨‍💻 Author

**Hari Kumar**
