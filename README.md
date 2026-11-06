# AI CRM Dashboard

<p align="center">
  <strong>A Modern Full-Stack Customer Relationship Management Platform</strong>
</p>

<p align="center">
  Built with MongoDB, Express.js, React.js, Node.js and Tailwind CSS.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/React-Frontend-61DAFB?style=flat-square&logo=react&logoColor=white" />
  <img src="https://img.shields.io/badge/Node.js-Backend-339933?style=flat-square&logo=nodedotjs&logoColor=white" />
  <img src="https://img.shields.io/badge/Express.js-Framework-black?style=flat-square&logo=express" />
  <img src="https://img.shields.io/badge/MongoDB-Database-47A248?style=flat-square&logo=mongodb&logoColor=white" />
  <img src="https://img.shields.io/badge/Tailwind_CSS-Styling-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white" />
</p>

---

## Overview

**AI CRM Dashboard** is a full-stack Customer Relationship Management application designed to provide a centralized platform for managing customer information, tracking business relationships, and organizing sales-related workflows.

The application follows a modern MERN stack architecture, combining a React-based frontend with a Node.js and Express.js backend, supported by MongoDB for persistent data storage.

The project focuses on building a scalable application structure, reusable components, maintainable backend services, and a responsive user experience.

## Key Features

- **CRM Dashboard:** Centralized interface for accessing CRM information.
- **Customer Management:** Organize and manage customer records.
- **Lead Management:** Structure and track potential business opportunities.
- **RESTful APIs:** Backend API architecture for frontend communication.
- **Database Integration:** MongoDB integration using Mongoose.
- **Responsive Interface:** Modern UI built with React and Tailwind CSS.
- **Error Handling:** Centralized backend error-handling middleware.
- **Environment Configuration:** Secure configuration through environment variables.
- **AI Integration:** Architecture intended to support AI-powered CRM functionality.

## Technology Stack

| Layer | Technology |
|---|---|
| Frontend | React.js |
| Styling | Tailwind CSS |
| Backend | Node.js |
| Server Framework | Express.js |
| Database | MongoDB |
| ODM | Mongoose |
| API Architecture | REST API |
| Development Tools | Git, GitHub, VS Code |

## Project Architecture

The application follows a modular client-server architecture.

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
│   └── server.js
│
├── frontend/
│   ├── src/
│   ├── public/
│   └── package.json
│
├── .gitignore
└── README.md
```

## Getting Started

Follow these instructions to set up the project locally.

### Prerequisites

Make sure you have the following installed:

- Node.js (LTS version)
- npm
- MongoDB Atlas account or local MongoDB
- Git

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
```

Navigate into the project:

```bash
cd YOUR-REPOSITORY
```

### 2. Backend Setup

Navigate to the backend directory:

```bash
cd backend
```

Install dependencies:

```bash
npm install
```

Create a `.env` file inside the backend directory:

```env
PORT=5000
NODE_ENV=development
CLIENT_URL=http://localhost:5173
MONGO_URI=your_mongodb_connection_string
```

Start the backend development server:

```bash
npm run dev
```

### 3. Frontend Setup

Open another terminal:

```bash
cd frontend
```

Install dependencies:

```bash
npm install
```

Start the frontend development server:

```bash
npm run dev
```

### 4. Access the Application

| Service | Local URL |
|---|---|
| Frontend | http://localhost:5173 |
| Backend | http://localhost:5000 |

## Environment Variables

| Variable | Description |
|---|---|
| PORT | Backend server port |
| NODE_ENV | Application environment |
| CLIENT_URL | Frontend origin for CORS |
| MONGO_URI | MongoDB connection string |

**Security Note:** Never commit `.env` files, database credentials, API keys, or other sensitive configuration to version control.

## Backend Engineering

The backend is organized into separate modules to improve maintainability and separation of concerns.

- **Config:** Database and application configuration.
- **Controllers:** Request handling and business logic coordination.
- **Models:** MongoDB schemas and data models.
- **Routes:** API endpoint definitions.
- **Middleware:** Request processing, authentication and error handling.
- **Services:** Reusable application-level business logic.
- **Utils:** Shared utilities and helper functions.

## Development Principles

The project is structured around the following engineering principles:

- Modular and maintainable code organization.
- Separation of frontend and backend responsibilities.
- Reusable UI and backend components.
- Centralized error handling.
- Environment-based configuration.
- Consistent API communication.
- Scalable application architecture.

## Roadmap

Potential future improvements:

- [ ] Authentication and authorization
- [ ] Role-based access control
- [ ] Advanced customer analytics
- [ ] AI-powered customer insights
- [ ] Automated lead scoring
- [ ] CRM activity tracking
- [ ] Real-time notifications
- [ ] Dashboard data visualization
- [ ] Automated testing
- [ ] Production deployment

## Contributing

Contributions, suggestions, and improvements are welcome.

1. Fork the repository.
2. Create a feature branch.
3. Implement your changes.
4. Commit your changes.
5. Open a Pull Request.

## License

This project is currently intended for educational and development purposes.

A formal open-source license can be added when the project is ready for public distribution.

---

<p align="center">
  <strong>Built with a focus on clean code, scalable architecture, and modern web development.</strong>
</p>

<p align="center">
  Developed with ❤️ using the MERN Stack.
</p>
