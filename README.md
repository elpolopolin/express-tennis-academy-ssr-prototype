# Tennis Academy Management (Prototype / V1)

> **⚠️ Project Status Notice:** > This repository contains the **initial prototype / early version** of a Tennis Academy management system. The actual, full-scale project is currently in active development, has migrated to a more advanced architecture, and is **privately hosted** as it is currently in production use by a real academy. 
> 
> This public repository serves solely as a showcase of the initial logical workflows, monolithic architecture, and early-stage integration of key features like Stripe payments and role-based authentication.

## 📖 About the Prototype
This is a monolithic Node.js web application built to handle the daily operations of a tennis academy. It utilizes Server-Side Rendering (SSR) via EJS to deliver dynamic views directly from the Express backend.

The system was designed to manage:
- **Students & Memberships:** Registration, profile management, and class assignments.
- **Classes:** Scheduling and tracking.
- **Billing & Payments:** End-to-end integration with Stripe for invoice generation and payment processing.
- **Role-based Access:** Differentiating between admin/staff capabilities and standard users via JWT.

## 🛠️ Tech Stack
- **Backend:** Node.js, Express.js
- **Frontend / Views:** EJS (Embedded JavaScript templates), HTML/CSS
- **Database:** MySQL
- **Authentication:** JWT (JSON Web Tokens), `bcrypt` for password hashing
- **Integrations:** Stripe API (Payments), `multer` (File uploads)

## 🏗️ Architecture & Historical Context
This prototype was built using a classic MVC (Model-View-Controller) pattern. As a monolithic application, both the API routes and the UI rendering logic reside within this single codebase. 

While this repository demonstrates strong foundational features (parameterized SQL queries, hashed storage, end-to-end payment flows), the private production version has since been refactored to include:
- Strict CI/CD pipelines and automated testing.
- Enhanced security middlewares and strict CORS/Cookie policies.
- Decoupled services (Microservices/API-first approach).

## 🚀 Running the Prototype Locally
*(Note: Since this is an archived prototype, you will need your own `.env` configurations to run it).*

1. Clone the repository: `git clone https://github.com/your-username/your-repo-name.git`
2. Install dependencies: `npm install`
3. Set up your `.env` file with your local MySQL credentials, JWT Secret, and Stripe test keys.
4. Run the server: `npm start`
