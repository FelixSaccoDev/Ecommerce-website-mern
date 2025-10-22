# 🛒 MERN Ecommerce

## Overview

**MERN Ecommerce** is a full-featured, **cloud-native ecommerce application** built with the **modern MERN stack (MongoDB, Express, React, Node.js)**.
It integrates **Sass for modular styling**, **Docker for containerized development**, and **Vercel for serverless cloud deployment**, following best practices in scalability, maintainability, and CI/CD workflows.

Developed by **Felix Sacco**, a **Fullstack Developer from the United States**, this project represents a production-grade implementation of today’s **modern web ecosystem** — combining flexible APIs, state management, cloud hosting, and developer-first tooling.

---

## ⚡ Highlights

* **🌐 Modern Fullstack Architecture** – Built with the MERN stack for seamless front-to-back integration
* **🎨 Scalable Styling with Sass (SCSS Modules)** – Component-based styles for maintainable UI development
* **🐳 Docker-Ready** – Fully containerized environment for consistent local and cloud deployment
* **☁️ Cloud Deployment (Vercel)** – Continuous serverless deployment with automatic scaling
* **🧠 Redux Toolkit + Thunk** – Predictable global state management with async data flow
* **📦 RESTful API Design** – Secure and modular backend powered by Express and MongoDB
* **🔐 Role-Based Access Control** – Separate experiences for Admins, Sellers, and Buyers
* **🧹 Code Quality First** – Prettier integration, ESLint, and consistent coding standards

## 🐳 Run Locally with Docker

You can run the entire application locally in a cloud-like environment using Docker Compose.

### 1. Clone the repository

```bash
git clone https://github.com/mohamedsamara/mern-ecommerce.git
cd mern-ecommerce
```

### 2. Configure environment variables

Edit the `docker-compose.yml` file and update:

* `MONGO_URI`
* `JWT_SECRET`

### 3. Build and start containers

```bash
docker-compose build
docker-compose up
```

> This spins up isolated containers for both **frontend** and **backend**, ensuring consistency across environments.

---

## 🌱 Database Seeding

Create an admin user for development or testing:

```bash
npm run seed:db [email@example.com] [password123]
```

See the [seed script](server/utils/seed.js) for details.

---

## ⚙️ Local Setup (Without Docker)

You can also run the project directly on your machine:

```bash
git clone https://github.com/mohamedsamara/mern-ecommerce.git
cd mern-ecommerce
npm install
npm run dev
```

---

## 🔧 Environment Configuration

Create `.env` files for both frontend and backend.
Use the provided examples for reference:

* [Client ENV Example](client/.env.example)
* [Server ENV Example](server/.env.example)

---

## ☁️ Cloud Deployment (Vercel)

The project is deployed to **Vercel**, leveraging its **serverless architecture** and **Git-based CI/CD** pipeline.

* Deploy both `client` and `server` from the same repository
* Configure each deployment’s root directory:

  * Frontend → `/client`
  * Backend → `/server`

Example configs:

* [client/vercel.json](client/vercel.json)
* [server/vercel.json](server/vercel.json)

> This setup ensures automatic build, deploy, and scaling from your GitHub main branch.

---

## 🧩 Tech Stack

| Category             | Technology                                         |
| -------------------- | -------------------------------------------------- |
| **Frontend**         | React, Redux Toolkit, Sass (SCSS Modules), Webpack |
| **Backend**          | Node.js, Express, REST API                         |
| **Database**         | MongoDB, Mongoose                                  |
| **Containerization** | Docker, Docker Compose                             |
| **Cloud Deployment** | Vercel (Serverless Functions)                      |
| **Version Control**  | Git, GitHub                                        |
| **Code Quality**     | Prettier, ESLint                                   |

---

## 🧹 Code Formatting (Prettier Configuration)

Inside `.vscode/settings.json`:

```json
{
  "editor.formatOnSave": true,
  "prettier.singleQuote": true,
  "prettier.arrowParens": "avoid",
  "prettier.jsxSingleQuote": true,
  "prettier.trailingComma": "none",
  "javascript.preferences.quoteStyle": "single"
}
```

---

## 👨‍💻 About the Developer

**Felix Sacco**
*Fullstack Developer – United States*

Building performant, cloud-ready web applications using **React**, **Node.js**, **Docker**, and **Sass**.
Focused on **scalable architecture**, **developer productivity**, and **modern cloud infrastructure**.

