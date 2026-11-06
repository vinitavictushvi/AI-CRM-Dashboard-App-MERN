# AI CRM Dashboard

### Intelligent Customer Relationship Management Platform

<p align="center">
  <strong>BUILD SMARTER RELATIONSHIPS. MAKE BETTER DECISIONS.</strong>
</p>

<p align="center">
  A modern full-stack CRM platform built to centralize customer management, streamline business workflows, and establish a foundation for AI-powered business intelligence.
</p>

<p align="center">
  ![Project Status](https://img.shields.io/badge/Project-In%20Development-2563EB?style=for-the-badge)
  ![Architecture](https://img.shields.io/badge/Architecture-Full--Stack-111827?style=for-the-badge)
  ![Stack](https://img.shields.io/badge/Stack-MERN-16A34A?style=for-the-badge)
</p>

<p align="center">
  ![React](https://img.shields.io/badge/React-Frontend-61DAFB?style=flat-square&logo=react&logoColor=black)
  ![Node.js](https://img.shields.io/badge/Node.js-Runtime-339933?style=flat-square&logo=nodedotjs&logoColor=white)
  ![Express](https://img.shields.io/badge/Express.js-Backend-000000?style=flat-square&logo=express)
  ![MongoDB](https://img.shields.io/badge/MongoDB-Database-47A248?style=flat-square&logo=mongodb&logoColor=white)
  ![Tailwind](https://img.shields.io/badge/Tailwind_CSS-Styling-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
  ![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
</p>

---

## Table of Contents

- [Overview](#-overview)
- [Product Vision](#-product-vision)
- [Core Modules](#-core-modules)
- [Technology Stack](#-technology-stack)
- [System Architecture](#-system-architecture)
- [Project Structure](#-project-structure)
- [Getting Started](#-getting-started)
- [Environment Configuration](#-environment-configuration)
- [Application Workflow](#-application-workflow)
- [Backend Engineering](#-backend-engineering)
- [API Documentation](#-api-documentation)
- [Security Considerations](#-security-considerations)
- [Development Roadmap](#-development-roadmap)
- [Contributing](#-contributing)
- [License](#-license)

---

## 01. Overview

**AI CRM Dashboard** is a full-stack Customer Relationship Management application developed using the MERN technology stack.

The project is designed to provide a centralized environment for managing customer information, organizing business relationships, tracking potential leads, and supporting data-driven business operations.

The application follows a modular client-server architecture with a React-based frontend, an Express.js backend, and MongoDB as its database layer.

The long-term objective is to integrate AI-powered capabilities into traditional CRM workflows, creating a smarter and more efficient business management experience.

### What Makes This Project Different?

- Modern full-stack JavaScript architecture.
- Modular backend organization.
- Dedicated frontend and backend environments.
- MongoDB-based data persistence.
- Centralized error-handling architecture.
- Scalable foundation for AI integrations.
- Maintainability-focused development approach.

## 02. Product Vision

The vision is to develop a unified CRM platform that makes customer relationship management more organized, intelligent, and accessible.

### Engineering Objectives

**Centralization**

Bring customer information and business workflows into one environment.

**Intelligence**

Create opportunities for AI-assisted customer insights and automation.

**Scalability**

Build a modular foundation that can evolve with additional features.

**Maintainability**

Follow structured development practices and separation of concerns.

**User Experience**

Deliver an intuitive, responsive, and consistent dashboard experience.

## 03. Core Modules

The platform is organized around the following functional areas.

| Module | Responsibility |
|---|---|
| Dashboard | Centralized CRM overview |
| Customer Management | Customer information and records |
| Lead Management | Lead organization and tracking |
| Analytics | Business performance insights |
| AI Intelligence | AI-assisted business workflows |
| User Management | User accounts and administration |
| API Layer | Frontend-backend communication |
| Database Layer | Persistent application data |

*These represent the intended product modules. Their implementation status depends on the current development progress.*

## 04. Technology Stack

The application uses the MERN ecosystem and supporting development tools.

### Frontend

| Technology | Purpose |
|---|---|
| React.js | Component-based UI |
| JavaScript | Application logic |
| Tailwind CSS | Utility-first styling |
| Vite | Frontend development and build tooling |

### Backend

| Technology | Purpose |
|---|---|
| Node.js | Server-side runtime |
| Express.js | HTTP server framework |
| Mongoose | MongoDB object modeling |
| dotenv | Environment configuration |
| CORS | Cross-origin request handling |
| Morgan | HTTP request logging |

### Database

| Technology | Purpose |
|---|---|
| MongoDB | NoSQL database |
| MongoDB Atlas | Cloud database hosting |

### Development Tools

- Visual Studio Code
- Git
- GitHub
- npm
- Postman

## 05. System Architecture

The application follows a layered client-server architecture.

### High-Level Architecture

```text
                 USER
                   |
                   v
          REACT FRONTEND
                   |
                   v
              HTTP / API
                   |
                   v
           EXPRESS SERVER
                   |
          +--------+--------+
          |        |        |
          v        v        v
        ROUTES  MIDDLEWARE  ERRORS
          |
          v
      CONTROLLERS
          |
          v
       SERVICES
          |
          v
       MONGOOSE
          |
          v
        MONGODB
```

### Architectural Responsibilities

**Presentation Layer**

React handles the user interface, reusable components, and client-side interactions.

**Routing Layer**

Express routes define the API endpoints and connect incoming requests to their respective handlers.

**Controller Layer**

Controllers coordinate request processing and application responses.

**Service Layer**

Services provide a dedicated location for reusable business logic.

**Data Layer**

Mongoose manages communication between the backend and MongoDB.

**Middleware Layer**

Middleware handles request processing, error management, and other cross-cutting concerns.

## 06. Project Structure

The repository is organized into separate frontend and backend applications.

```text
AI-CRM-DASHBOARD/
│
├── backend/
│   │
│   ├── config/
│   │   └── db.js
│   │
│   ├── controllers/
│   │
│   ├── middleware/
│   │   └── error.middleware.js
│   │
│   ├── models/
│   │
│   ├── routes/
│   │
│   ├── services/
│   │
│   ├── utils/
│   │   ├── ApiError.js
│   │   └── asyncHandler.js
│   │
│   ├── .env
│   ├── package.json
│   ├── package-lock.json
│   └── server.js
│
├── frontend/
│   │
│   └── ai-crm-dashboard/
│       │
│       ├── public/
│       ├── src/
│       ├── node_modules/
│       ├── .env.example
│       ├── .gitignore
│       ├── eslint.config.js
│       ├── index.html
│       ├── package.json
│       ├── package-lock.json
│       └── README.md
│
└── README.md
```

### Backend Directory Responsibilities

| Directory | Responsibility |
|---|---|
| config | Database and application configuration |
| controllers | Request handling |
| middleware | Request processing and error handling |
| models | Database schemas |
| routes | API endpoint definitions |
| services | Application business logic |
| utils | Reusable utilities and helpers |

### Frontend Directory Responsibilities

| Directory | Responsibility |
|---|---|
| public | Static assets |
| src | Main React application source |
| index.html | Frontend entry HTML |
| eslint.config.js | Code quality configuration |

## 07. Getting Started

Follow the instructions below to run the project locally.

### Prerequisites

Ensure the following tools are installed:

- Node.js (LTS)
- npm
- Git
- MongoDB Atlas account or local MongoDB instance
- Visual Studio Code

### Step 1 — Clone the Repository

```bash
git clone https://github.com/vinitavictushvi/AI-CRM-DASHBOARD-MERN.git
```

Navigate into the project:

```bash
cd AI-CRM-DASHBOARD
```

### Step 2 — Backend Installation

Open a terminal:

```bash
cd backend
```

Install dependencies:

```bash
npm install
```

### Step 3 — Backend Environment Setup

Create a `.env` file inside the backend directory.

```env
PORT=5000
NODE_ENV=development
CLIENT_URL=http://localhost:5173

MONGO_URI=your_mongodb_connection_string
```

Replace the MongoDB connection string with your actual database URI.

### Step 4 — Start Backend Server

```bash
npm run dev
```

Backend development server:

```text
http://localhost:5000
```

The backend package must have a development script configured for this command.

### Step 5 — Frontend Installation

Open a second terminal from the project root:

```bash
cd frontend/ai-crm-dashboard
```

Install dependencies:

```bash
npm install
```

### Step 6 — Start Frontend

```bash
npm run dev
```

Vite development server:

```text
http://localhost:5173
```

### Step 7 — Access the Application

| Application | URL |
|---|---|
| Frontend | http://localhost:5173 |
| Backend | http://localhost:5000 |

---

## 08. Environment Configuration

Environment variables are used to keep application configuration separate from source code.

### Backend Variables

| Variable | Description |
|---|---|
| PORT | Backend server port |
| NODE_ENV | Application environment |
| CLIENT_URL | Frontend origin |
| MONGO_URI | MongoDB connection string |

### Frontend Configuration

If the frontend needs to communicate with the backend through an environment variable, configure a Vite variable in the frontend `.env` file.

```env
VITE_API_URL=http://localhost:5000
```

Access it in frontend code using:

```javascript
import.meta.env.VITE_API_URL
```

Never expose private server credentials or secret API keys through frontend environment variables.

---

## 09. Application Workflow

The expected application request lifecycle is:

1. The user interacts with the React frontend.
2. The frontend sends an HTTP request to the backend.
3. Express receives the request.
4. Middleware processes the request.
5. The appropriate route forwards the request to its controller.
6. The controller coordinates application logic.
7. Services perform the required operations.
8. Mongoose communicates with MongoDB.
9. The backend returns a structured HTTP response.
10. The frontend updates the interface.

This separation makes the system easier to maintain, test, and extend.

## 10. Backend Engineering

The backend is designed around modular development principles.

### Database Connectivity

MongoDB connectivity is managed through a dedicated configuration module.

**File:** `backend/config/db.js`

### Error Handling

Centralized error-handling middleware provides a consistent mechanism for processing application errors.

**File:** `backend/middleware/error.middleware.js`

### Utility Layer

Shared utilities are maintained separately to reduce duplicated code.

Current utility files include:

- `ApiError.js`
- `asyncHandler.js`

### Logging

Morgan is used for HTTP request logging during development.

### Application Initialization

The main Express application and database startup process are managed through:

`backend/server.js`

## 11. API Documentation

The backend is structured to support resource-oriented REST API development.

### Planned API Resource Structure

| Endpoint | Resource |
|---|---|
| `/api/auth` | Authentication |
| `/api/users` | User management |
| `/api/customers` | Customer management |
| `/api/leads` | Lead management |
| `/api/analytics` | Analytics |

### HTTP Methods

| Method | Purpose |
|---|---|
| GET | Retrieve resources |
| POST | Create resources |
| PUT | Replace or update resources |
| PATCH | Partially update resources |
| DELETE | Remove resources |

The endpoint groups above are proposed API organization, not a claim that these routes are already implemented.

## 12. Security Considerations

Security is an important part of building production-ready applications.

The following practices are recommended as the project evolves:

- Store sensitive credentials in environment variables.
- Never commit `.env` files.
- Validate incoming request data.
- Implement authentication before exposing protected resources.
- Apply role-based authorization where required.
- Restrict CORS to trusted origins.
- Use secure password hashing.
- Avoid exposing internal server errors in production.
- Keep dependencies updated.
- Protect database access through appropriate network and credential restrictions.

## 13. Development Roadmap

The project is being developed incrementally.

### Phase 01 — Foundation

- [x] Backend folder structure
- [x] Express application setup
- [x] MongoDB connection module
- [x] CORS configuration
- [x] Centralized error-handling foundation
- [ ] Frontend-backend integration

### Phase 02 — Core CRM Features

- [ ] User authentication
- [ ] Customer management
- [ ] Lead management
- [ ] Sales pipeline management
- [ ] Customer activity tracking

### Phase 03 — AI Integration

- [ ] AI-powered customer insights
- [ ] Intelligent lead scoring
- [ ] AI-assisted recommendations
- [ ] Workflow automation
- [ ] Smart business analytics

### Phase 04 — Advanced Engineering

- [ ] Role-based access control
- [ ] Advanced dashboard analytics
- [ ] Automated testing
- [ ] API documentation
- [ ] Performance optimization
- [ ] Production deployment
- [ ] Monitoring and logging

## 14. Quality Engineering

The long-term engineering objective is to maintain a reliable and maintainable codebase.

Planned engineering practices include:

| Area | Standard |
|---|---|
| Code Quality | ESLint |
| Code Formatting | Prettier |
| API Testing | Postman |
| Unit Testing | Automated test suites |
| Integration Testing | API and database testing |
| Version Control | Git |
| Documentation | Markdown |

## 15. Contributing

Contributions, improvements, and technical feedback are welcome.

### Contribution Workflow

1. Fork the repository.
2. Create a new feature branch.
3. Implement your changes.
4. Test the implementation.
5. Commit with a descriptive message.
6. Open a Pull Request.

Example:

```bash
git checkout -b feature/customer-management

git add .

git commit -m "feat: add customer management module"

git push origin feature/customer-management
```

## 16. License

No open-source license has been specified yet.

A formal license will be added when the project is ready for public distribution.

Until then, all rights remain with the project owner.

---

## Engineering Philosophy

Building a meaningful software product requires more than implementing features.

It requires thoughtful architecture, maintainable code, reliable data management, and a commitment to continuous improvement.

**AI CRM Dashboard** is being developed with these principles at its core.

<p align="center">
  <strong>ENGINEERED FOR CLARITY.</strong>
  <br/>
  <strong>DESIGNED FOR SCALE.</strong>
  <br/>
  <strong>BUILT FOR WHAT'S NEXT.</strong>
</p>

<p align="center">
  Developed using the MERN Stack.
</p>
