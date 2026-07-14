# 🚀 InnoSync – Student Collaboration Platform

<p align="center">
  <img src="https://img.shields.io/badge/Frontend-React%20(Vite)-61DAFB?style=for-the-badge&logo=react" />
  <img src="https://img.shields.io/badge/Backend-FastAPI-009688?style=for-the-badge&logo=fastapi" />
  <img src="https://img.shields.io/badge/Database-MongoDB-47A248?style=for-the-badge&logo=mongodb" />
  <img src="https://img.shields.io/badge/License-MIT-blue?style=for-the-badge" />
</p>

<p align="center">
  <strong>A modern full-stack platform that empowers students to collaborate on academic projects, manage teams, share resources, and communicate efficiently—all in one place.</strong>
</p>

---

# 📖 Table of Contents

- Overview
- Problem Statement
- Solution
- Key Features
- System Architecture
- Tech Stack
- Folder Structure
- Installation
- Configuration
- Running the Project
- API Overview
- Database Schema
- Screenshots
- Future Scope
- Contributors
- License

---

# 📌 Overview

InnoSync is a full-stack web application designed to simplify collaboration among students working on academic, research, hackathon, and extracurricular projects.

Students often use multiple disconnected platforms like WhatsApp, Google Drive, Email, GitHub, and spreadsheets to manage projects. This fragmented workflow creates communication gaps, inefficient resource management, and difficulty tracking project progress.

InnoSync solves these challenges by providing a centralized collaboration platform where students can create projects, manage teams, communicate, and share resources seamlessly.

---

# 🎯 Problem Statement

Student teams commonly face several challenges:

- Difficulty finding teammates with required skills
- Unorganized communication across multiple apps
- Scattered project files
- Poor task coordination
- Lack of project visibility
- Difficulty tracking deadlines
- Manual project management

These issues become even more significant during hackathons, semester projects, and final-year projects.

---

# 💡 Solution

InnoSync provides a unified platform that enables students to:

- Create and manage projects
- Build collaborative teams
- Upload and organize project resources
- Track project activities
- Maintain individual student profiles
- Securely authenticate users
- Manage all collaboration from one dashboard

---

# ✨ Features

## 🔐 User Authentication

- User Registration
- Secure Login
- Logout
- Password validation
- Session management

---

## 👤 Student Profile

Every student has a personalized profile containing:

- Name
- Email
- Department
- Skills
- Biography
- Profile Picture
- Current Projects

---

## 📂 Project Management

Students can:

- Create new projects
- Edit project details
- Delete projects
- View all projects
- Search projects
- Filter projects

Each project includes:

- Title
- Description
- Required Skills
- Team Members
- Project Status
- Deadline

---

## 👥 Team Collaboration

Project owners can:

- Invite members
- Remove members
- Assign responsibilities
- View contributors
- Manage collaboration

---

## 📁 Resource Sharing

Members can upload:

- PDFs
- PPTs
- Images
- ZIP files
- Documents

All project resources remain organized within the project.

---

## 💬 Communication

Members can communicate within the platform to discuss project updates and coordinate work without relying on third-party messaging applications.

---

## 📊 Dashboard

The dashboard provides:

- Active Projects
- Completed Projects
- Pending Projects
- Recent Activities
- Team Overview
- Project Statistics

---

## 🔔 Notifications

Receive notifications for:

- New invitations
- Project updates
- Uploaded resources
- Team activities

---

# 🏗️ System Architecture

```
                +-----------------------+
                |      React Frontend   |
                +-----------+-----------+
                            |
                     REST API Requests
                            |
                +-----------v-----------+
                |      FastAPI Server   |
                +-----------+-----------+
                            |
              Business Logic & Validation
                            |
                +-----------v-----------+
                |       MongoDB         |
                +-----------------------+
```

---

# 🛠️ Tech Stack

## Frontend

- React.js
- Vite
- HTML5
- CSS3
- JavaScript (ES6+)

---

## Backend

- FastAPI
- Python
- Pydantic
- Uvicorn

---

## Database

- MongoDB
- PyMongo

---

## Tools

- Git
- GitHub
- VS Code
- Postman

---

# 📁 Project Structure

```
InnoSync/
│
├── frontend/
│   ├── public/
│   ├── src/
│   │
│   ├── assets/
│   ├── components/
│   ├── pages/
│   ├── services/
│   ├── App.jsx
│   └── main.jsx
│
├── backend/
│   ├── routes/
│   ├── models/
│   ├── auth/
│   ├── database/
│   ├── utils/
│   ├── main.py
│   ├── requirements.txt
│   └── .env
│
├── README.md
└── LICENSE
```

---

# ⚙️ Installation

## Clone Repository

```bash
git clone https://github.com/yourusername/InnoSync.git
```

```
cd InnoSync
```

---

## Backend Setup

Create Virtual Environment

```bash
python -m venv venv
```

Activate Environment

Windows

```bash
venv\Scripts\activate
```

Linux / macOS

```bash
source venv/bin/activate
```

Install Dependencies

```bash
pip install -r requirements.txt
```

Run Backend

```bash
uvicorn main:app --reload
```

---

## Frontend Setup

```bash
cd frontend
```

Install Packages

```bash
npm install
```

Run Application

```bash
npm run dev
```

---

# ⚙️ Environment Variables

Create a `.env` file inside the backend directory.

```env
MONGO_URI=mongodb://localhost:27017
DATABASE_NAME=innosync
SECRET_KEY=your_secret_key
ALGORITHM=HS256
ACCESS_TOKEN_EXPIRE_MINUTES=60
```

---

# 🌐 API Overview

| Method | Endpoint | Description |
|----------|----------------|---------------------------|
| POST | /register | Register user |
| POST | /login | Login |
| GET | /users | Get users |
| POST | /projects | Create project |
| GET | /projects | Get all projects |
| GET | /projects/{id} | Get project |
| PUT | /projects/{id} | Update project |
| DELETE | /projects/{id} | Delete project |

---

# 🗄️ Database Collections

## Users

```json
{
  "_id": "...",
  "name": "John",
  "email": "john@example.com",
  "password": "...",
  "skills": ["Python","React"],
  "bio": "...",
  "profilePicture": "..."
}
```

---

## Projects

```json
{
  "_id": "...",
  "title": "Student Portal",
  "description": "...",
  "owner": "...",
  "members": [],
  "deadline": "...",
  "status": "Active"
}
```

---

# 📈 Future Enhancements

- JWT Authentication
- Role-Based Access Control
- Real-time Chat (WebSockets)
- Kanban Task Board
- Calendar Integration
- Email Notifications
- AI Team Recommendation System
- GitHub Repository Integration
- Project Analytics Dashboard
- Mobile Application
- Docker Deployment
- Cloud Deployment
- CI/CD Pipeline

---

# 🎯 Learning Outcomes

This project demonstrates:

- Full Stack Development
- REST API Development
- Database Design
- Authentication & Authorization
- CRUD Operations
- Frontend–Backend Integration
- API Testing
- Git & GitHub Workflow
- Team Collaboration
- Software Engineering Practices

---

# 📸 Screenshots

Add screenshots of:

- Login Page
- Registration
- Dashboard
- Project List
- Project Details
- Profile
- Team Management
- Resource Upload

Example:

```
docs/screenshots/login.png
docs/screenshots/dashboard.png
docs/screenshots/projects.png
```

---

# 🤝 Contributors

- **Shweta Gaidhani** – Backend Development
- **Team Members** – Frontend Development, Testing & Documentation

---

# 📄 License

This project is licensed under the MIT License.

---

# 🌟 Acknowledgements

Special thanks to:

- Faculty mentors
- Project teammates
- Open-source community
- FastAPI
- React
- MongoDB

---

<p align="center">
Built using React, FastAPI & MongoDB
</p>