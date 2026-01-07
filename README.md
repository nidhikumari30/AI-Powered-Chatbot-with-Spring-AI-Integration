# 🤖 AI-Powered Chatbot with Spring AI Integration

> **An Intelligent Conversational AI Application** | A Full-Stack College Project  
> Built with React, Spring Boot, and Spring AI Framework

![Project Status](https://img.shields.io/badge/Status-In%20Development-brightgreen)
![Java Version](https://img.shields.io/badge/Java-11%2B-blue)
![React Version](https://img.shields.io/badge/React-17.0.2-61DAFB?logo=react)
![License](https://img.shields.io/badge/License-MIT-green)

---

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [User Roles & Capabilities](#user-roles--capabilities)
- [Installation & Setup](#installation--setup)
- [Running the Application](#running-the-application)
- [Database Configuration](#database-configuration)
- [API Documentation](#api-documentation)
- [Project Architecture](#project-architecture)
- [Contributing](#contributing)
- [License](#license)
- [Developer Info](#developer-info)

---

## Overview

**AI-Powered Chatbot with Spring AI Integration** is a full-stack web application that demonstrates the integration of AI technologies into modern web applications. This college project showcases how to build an intelligent conversational interface where users can interact with an AI-powered chatbot using natural language.

The application consists of:
- **Frontend**: A responsive React-based chat interface for seamless user interactions
- **Backend**: A Spring Boot REST API powered by Spring AI for intelligent response generation
- **Database**: MySQL for storing user data and conversation history
- **AI Engine**: Spring AI Framework for natural language processing and AI model integration

### Purpose
This project serves as a learning platform for understanding:
- Full-stack web application development
- AI and machine learning integration in web apps
- RESTful API design with Spring Boot
- Modern React frontend development
- Authentication and authorization mechanisms
- Real-time communication patterns

---

## ✨ Features

### Core Features
- 💬 **AI Conversational Interface** - Chat naturally with an intelligent chatbot powered by Spring AI
- 🧠 **Spring AI Integration** - Advanced language models for intelligent responses
- 🔐 **Secure Authentication** - JWT-based authentication for user security
- 👤 **User Accounts** - Create and manage user profiles
- 💾 **Conversation History** - Automatically save and retrieve chat conversations
- ⚡ **Real-Time Responses** - Get instant AI-powered answers

### Advanced Features
- 📧 **Email Notifications** - Email confirmation for important actions
- 🔄 **Session Management** - Automatic token refresh for seamless experience
- 🎨 **Modern UI** - Beautiful, responsive interface built with React and Semantic UI
- 📱 **Cross-Device Support** - Works on desktop and mobile devices
- 🧪 **Comprehensive Testing** - Jest and Spring Boot Testing frameworks
- 📊 **API Documentation** - Auto-generated Swagger/OpenAPI documentation

---

## 🛠 Tech Stack

### Frontend
| Technology | Version | Purpose |
|-----------|---------|---------|
| **React** | 17.0.2 | UI Framework |
| **React Router** | 6.0+ | Client-side routing |
| **Semantic UI React** | Latest | UI Component Library |
| **Axios** | 0.24.0 | HTTP Client |
| **Formik** | 2.2.9 | Form Management |
| **Styled Components** | 5.3.3 | CSS-in-JS Styling |
| **Jest** | Latest | Testing Framework |

### Backend
| Technology | Version | Purpose |
|-----------|---------|---------|
| **Spring Boot** | 2.4.2 | Framework |
| **Spring Web** | Latest | REST API |
| **Spring Security** | Latest | Authentication & Authorization |
| **Spring Data JPA** | Latest | Database ORM |
| **Spring AI** | Latest | AI/ML Integration |
| **MySQL** | 8.0+ | Database |
| **Maven** | Latest | Build Tool |
| **JWT** | Latest | Token-based Auth |
| **Swagger/OpenAPI** | 1.6.4 | API Documentation |

### DevOps & Tools
- **Docker** - Container orchestration
- **Docker Compose** - Multi-container orchestration
- **Git** - Version control

---

## 📂 Project Structure

```
📦 AI-Powered-Chatbot-with-Spring-AI-Integration
│
├── 📁 react-frontend                 (React Single-Page Application)
│   ├── public/                       (Static assets)
│   │   ├── index.html               (Entry HTML)
│   │   └── manifest.json            (PWA manifest)
│   │
│   ├── src/                         (Source code)
│   │   ├── components/              (React components)
│   │   │   ├── protectedRoutes/     (Private route components)
│   │   │   ├── root/                (Root layout components)
│   │   │   └── fragments/           (Reusable UI fragments)
│   │   │
│   │   ├── api/                     (API Service Layer)
│   │   │   ├── authentication/      (Login, signup services)
│   │   │   ├── hobby/               (Hobby/offer services)
│   │   │   ├── users/               (User management services)
│   │   │   └── test/                (Test services)
│   │   │
│   │   ├── css/                     (CSS Modules)
│   │   │   ├── Account.module.css
│   │   │   ├── Forms.module.css
│   │   │   └── ...
│   │   │
│   │   ├── img/                     (Images & assets)
│   │   ├── __test__/                (Test files)
│   │   ├── App.js                   (Root component)
│   │   ├── index.js                 (Entry point)
│   │   └── babel.config.js          (Babel configuration)
│   │
│   ├── package.json                 (NPM dependencies)
│   └── jest.config.js               (Jest testing config)
│
├── 📁 spring-backend                 (Spring Boot REST API)
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/                (Java source code)
│   │   │   │   └── backend/
│   │   │   │       ├── controller/  (REST Controllers)
│   │   │   │       ├── service/     (Business Logic)
│   │   │   │       ├── repository/  (Database Layer - JPA)
│   │   │   │       ├── model/       (Entity classes)
│   │   │   │       ├── security/    (JWT & Security config)
│   │   │   │       └── exception/   (Exception handlers)
│   │   │   │
│   │   │   └── resources/
│   │   │       ├── application.properties    (Config)
│   │   │       └── application-dev.properties (Dev config)
│   │   │
│   │   └── test/                    (Test classes)
│   │
│   ├── pom.xml                      (Maven dependencies)
│   ├── docker-compose.yml           (Docker services)
│   ├── Dockerfile                   (Container image)
│   ├── mvnw                         (Maven wrapper)
│   └── mvnw.cmd                     (Maven wrapper Windows)
│
├── README.md                         (This file)
└── LICENSE                           (MIT License)
```

---

## 👥 User Roles & Capabilities

### 1. **Guest User**
- Browse public information
- View chatbot interface (read-only)
- Access landing page

### 2. **Registered User**
- Create account with email verification
- Access full chatbot functionality
- Chat with AI assistant
- View conversation history
- Update profile information
- Logout securely

### 3. **Business User** (if applicable)
- Register business account
- Create/manage business profile
- View analytics (optional feature)
- Access admin dashboard

---

## 🚀 Installation & Setup

### Prerequisites
Ensure you have the following installed:

```bash
# Core Requirements
- Java Development Kit (JDK) 11+
- Node.js 16+ and npm 8+
- MySQL Database Server 8.0+
- Git

# Optional (for Docker setup)
- Docker Desktop 20.10+
- Docker Compose 1.29+
```

### Step 1: Clone the Repository

```bash
git clone https://github.com/nidhikumari30/AI-Powered-Chatbot-with-Spring-AI-Integration.git
cd AI-Powered-Chatbot-with-Spring-AI-Integration
```

### Step 2: Setup Frontend

```bash
# Navigate to frontend directory
cd react-frontend

# Install dependencies
npm install

# Create environment file (optional)
echo "REACT_APP_API_BASE_URL=http://localhost:8080" > .env
```

### Step 3: Setup Backend

```bash
# Navigate to backend directory
cd ../spring-backend

# If using Docker (recommended):
docker-compose up --build

# OR manually:
# Make sure MySQL is running
# Update application.properties with your DB credentials
./mvnw clean install
```

---

## ▶️ Running the Application

### Option 1: Using Docker Compose (Recommended)

```bash
# From project root
cd spring-backend
docker-compose up --build

# In a new terminal, start frontend
cd react-frontend
npm start
```

**Access Points:**
- Frontend: http://localhost:3000
- Backend API: http://localhost:8080
- API Docs: http://localhost:8080/swagger-ui/index.html

### Option 2: Manual Setup

#### Start Backend:
```bash
cd spring-backend
./mvnw spring-boot:run
```
Backend runs at: http://localhost:8080

#### Start Frontend (in new terminal):
```bash
cd react-frontend
npm start
```
Frontend runs at: http://localhost:3000

### Running Tests

```bash
# Frontend tests
cd react-frontend
npm test

# Backend tests
cd spring-backend
./mvnw test
```

---

## 🗄️ Database Configuration

### Prerequisites
- MySQL Server 8.0+ installed and running

### Setup Steps

1. **Create Database:**
```sql
CREATE DATABASE chatbot_db;
USE chatbot_db;
```

2. **Configure Backend** (`spring-backend/src/main/resources/application.properties`):
```properties
# Database Configuration
spring.datasource.url=jdbc:mysql://localhost:3306/chatbot_db
spring.datasource.username=root
spring.datasource.password=your_password
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver

# JPA Configuration
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=false
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQL8Dialect

# JWT Configuration
app.jwt.secret=your_secret_key_min_256_bits_long
app.jwt.expiration=86400000

# Email Configuration (optional)
spring.mail.host=smtp.gmail.com
spring.mail.port=587
spring.mail.username=your_email@gmail.com
spring.mail.password=your_app_password
spring.mail.properties.mail.smtp.auth=true
spring.mail.properties.mail.smtp.starttls.enable=true
```

3. **Verify Connection:**
```bash
cd spring-backend
./mvnw spring-boot:run
# Check logs for "Started Application in X seconds"
```

### Schema Details
Tables created automatically:
- `users` - User account information
- `conversation` - Chat messages and history
- `roles` - User role definitions
- `user_roles` - User-role mapping

---

## 📚 API Documentation

### Accessing API Docs

When the backend is running, visit:
```
http://localhost:8080/swagger-ui/index.html
```

### Key Endpoints

#### Authentication
```
POST   /api/auth/signup        - Register new user
POST   /api/auth/login         - User login
POST   /api/auth/refresh       - Refresh JWT token
POST   /api/auth/logout        - User logout
```

#### Chat/Chatbot
```
POST   /api/chat/message       - Send message to chatbot
GET    /api/chat/history       - Get conversation history
DELETE /api/chat/conversation  - Clear conversation
```

#### User Management
```
GET    /api/users/profile      - Get user profile
PUT    /api/users/profile      - Update user profile
GET    /api/users/{id}         - Get user by ID
DELETE /api/users/{id}         - Delete user account
```

### Authentication
All secured endpoints require JWT token in header:
```
Authorization: Bearer <your_jwt_token>
```

**To get a token:**
1. Register: POST `/api/auth/signup`
2. Login: POST `/api/auth/login`
3. Use returned token in Authorization header

---

## 🏗️ Project Architecture

### Architecture Pattern: **Layered Architecture**

```
┌─────────────────────────────────────┐
│     Presentation Layer (React)      │
│    - UI Components                  │
│    - Routing & State Management     │
└─────────────────────────────────────┘
              ↓ (HTTP/REST)
┌─────────────────────────────────────┐
│       API Layer (Spring Web)        │
│    - Controllers                    │
│    - Request/Response Handling      │
└─────────────────────────────────────┘
              ↓
┌─────────────────────────────────────┐
│    Business Logic Layer             │
│    - Services                       │
│    - AI/Chatbot Logic               │
│    - Spring AI Integration          │
└─────────────────────────────────────┘
              ↓
┌─────────────────────────────────────┐
│   Persistence Layer (Spring Data)   │
│    - Repositories (JPA)             │
│    - Database Operations            │
└─────────────────────────────────────┘
              ↓
┌─────────────────────────────────────┐
│      Database Layer (MySQL)         │
│    - Tables & Relationships         │
└─────────────────────────────────────┘
```

### Data Flow

1. **User Request**: Frontend sends request to API
2. **Controller**: Spring controller receives and validates request
3. **Service**: Business logic processes the request
4. **AI Processing**: Spring AI generates intelligent responses
5. **Repository**: Data is persisted to MySQL
6. **Response**: JSON response sent back to frontend
7. **UI Update**: React component updates with new data

---

## 🤝 Contributing

We welcome contributions! Here's how to get involved:

### Guidelines
1. **Fork** the repository on GitHub
2. **Clone** your fork locally
3. **Create** a feature branch: `git checkout -b feature/amazing-feature`
4. **Make** your changes with clear commit messages
5. **Write** tests for new functionality
6. **Commit**: `git commit -m 'Add amazing feature'`
7. **Push**: `git push origin feature/amazing-feature`
8. **Open** a Pull Request with detailed description

### Code Standards
- Follow Java naming conventions (camelCase for variables/methods, PascalCase for classes)
- Follow React/JSX best practices
- Write meaningful commit messages
- Include comments for complex logic
- Test your code before pushing

### Reporting Issues
Found a bug? Have a suggestion? Please open an issue with:
- Clear description of the problem
- Steps to reproduce
- Expected vs actual behavior
- Screenshots/logs if applicable

---

## 📄 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

You are free to:
- ✅ Use the code for personal or commercial projects
- ✅ Modify and distribute the code
- ✅ Use it in private applications

With conditions:
- Include the license and copyright notice

---

## 👩‍💻 Developer Info

### Developed by

**Nidhi Kumari**

**Contact & Social:**
- 📧 **Email**: [nidhikumari934181@gmail.com](mailto:nidhikumari934181@gmail.com)
- 🔗 **LinkedIn**: [linkedin.com/in/nidhi-kumari-4648692b2](https://linkedin.com/in/nidhi-kumari-4648692b2)
- 🐙 **GitHub**: [github.com/nidhikumari30](https://github.com/nidhikumari30)

### Project Details
- **Created**: January 2025
- **Type**: Full-Stack College Project
- **Status**: Active Development

---

## 📞 Support & Feedback

For questions, issues, or feedback:
1. Check existing [issues](https://github.com/nidhikumari30/AI-Powered-Chatbot-with-Spring-AI-Integration/issues)
2. Open a new issue with detailed information
3. Contact via email: nidhikumari934181@gmail.com

---

## 🙏 Acknowledgments

- Spring AI Framework team for the AI integration capabilities
- React community for excellent documentation
- Spring Boot community for robust backend framework
- All contributors and testers

---

<div align="center">

### Made with ❤️ and ☕ for learning and innovation

**Give this project a ⭐ if you found it helpful!**

</div>


