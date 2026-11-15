<div align="center">

```text
  ███████╗██╗  ██╗ █████╗ ██████╗ ███████╗███╗   ██╗
  ██╔════╝██║  ██║██╔══██╗██╔══██╗██╔════╝████╗  ██║
  ███████╗███████║███████║██║  ██║█████╗  ██╔██╗ ██║
  ╚════██║██╔══██║██╔══██║██║  ██║██╔══╝  ██║╚██╗██║
  ███████║██║  ██║██║  ██║██████╔╝███████╗██║ ╚████║
  ╚══════╝╚═╝  ╚═╝╚═╝  ╚═╝╚═════╝ ╚══════╝╚═╝  ╚═══╝
```

# SHADEN

### *Own the Unseen.*

**A Full-Stack Streetwear E-Commerce Platform Built for Modern Web Standards**

<p align="center">
  <a href="https://github.com/subhasankarsahu/shaden">
    <img src="https://img.shields.io/badge/Status-In%20Active%20Development-blue?style=for-the-badge&logo=git&logoColor=white&color=2563EB&labelColor=0F172A" alt="Development Status" />
  </a>
  <a href="https://github.com/subhasankarsahu/shaden/blob/main/LICENSE">
    <img src="https://img.shields.io/badge/License-MIT-blue?style=for-the-badge&color=2563EB&labelColor=0F172A" alt="License" />
  </a>
  <a href="#">
    <img src="https://img.shields.io/badge/Frontend-React%2019%20%7C%20Vite-61DAFB?style=for-the-badge&logo=react&logoColor=white&color=0284C7&labelColor=0F172A" alt="Frontend React 19" />
  </a>
  <a href="#">
    <img src="https://img.shields.io/badge/Backend-Express.js%20%7C%20Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white&color=16A34A&labelColor=0F172A" alt="Backend Express" />
  </a>
  <a href="#">
    <img src="https://img.shields.io/badge/Database-PostgreSQL%20%7C%20Prisma-4169E1?style=for-the-badge&logo=postgresql&logoColor=white&color=3B82F6&labelColor=0F172A" alt="Database PostgreSQL" />
  </a>
</p>

<p align="center">
  <img src="https://skillicons.dev/icons?i=react,vite,js,nodejs,express,postgres,prisma,git,github,postman,docker" alt="SHADEN Tech Stack" />
</p>

<p align="center">
  SHADEN bridges underground urban aesthetics with uncompromising software engineering fundamentals.
  <br />
  Engineered from scratch to demonstrate relational data integrity, robust RESTful APIs, secure auth workflows, and responsive client architectures.
</p>

---

</div>

## Table of Contents

- [About the Project](#about-the-project)
- [Project Objectives](#project-objectives)
- [Key Features](#key-features)
  - [Customer Storefront Features](#customer-storefront-features)
  - [Admin Dashboard Features](#admin-dashboard-features)
  - [Infrastructure and Repository Hygiene](#infrastructure-and-repository-hygiene)
- [Technology Stack](#technology-stack)
- [System Architecture](#system-architecture)
- [Project Directory Structure](#project-directory-structure)
- [Planned Database Schema](#planned-database-schema)
- [Application Workflow](#application-workflow)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Local Installation](#local-installation)
  - [Environment Variables](#environment-variables)
  - [Running the Application](#running-the-application)
- [API Specification (Planned)](#api-specification-planned)
- [Testing Strategy](#testing-strategy)
- [Security Architecture](#security-architecture)
- [Development Roadmap](#development-roadmap)
- [Contributing Guidelines](#contributing-guidelines)
- [License](#license)
- [Acknowledgements](#acknowledgements)

---

## About the Project

**SHADEN** is a full-stack e-commerce platform designed specifically for the streetwear and contemporary urban apparel vertical. The project goes beyond surface-level templates by focusing deliberately on clean architecture, end-to-end data modeling, relational consistency, and defense-in-depth security principles.

Rather than relying on plug-and-play third-party storefront builders or opaque boilerplates, SHADEN is constructed modularly to showcase how real-world commercial web applications handle:
- Complex catalog filtering, category nesting, and inventory variants (size, color, SKU).
- ACID-compliant transactional consistency across orders, payments, and stock allocations.
- Stateless token-based authentication and role-based access control (RBAC).
- Decoupled client-server communication via a predictable RESTful JSON API.

---

## Project Objectives

1. **Demonstrate Clean Engineering Practices:** Maintain strict separation of concerns through layered backend design (Routes $\rightarrow$ Middleware $\rightarrow$ Controllers $\rightarrow$ Services $\rightarrow$ Database).
2. **Relational Data Integrity:** Model real-world e-commerce entities in PostgreSQL with proper foreign key constraints, indexes, cascade policies, and migration tracking.
3. **Robust Security Posture:** Implement industry-standard security headers, request sanitization, CORS restrictions, rate-limiting, secure password hashing (`bcrypt`), and token lifecycle management (`JWT`).
4. **Deterministic Version Control:** Maintain impeccable Git hygiene, explicit `.gitignore` boundaries, semantic branch conventions, and zero-leakage policies for secrets and local tool caches.
5. **Production-Ready Deployment Foundations:** Scaffold codebases that cleanly decouple environment configuration from application logic, paving the way for Docker containerization and cloud deployment.

---

## Key Features

The following sections reflect the technical capability breakdown and current implementation status across all domains.

> **Status Legend:**  
> ✅ **Implemented:** Fully initialized and verified in repository code.  
> 🔄 **In Progress:** Scaffolding or configuration present; business logic under active development.  
> 📋 **Planned:** Architected and scheduled in the project roadmap.

### Customer Storefront Features

| Capability | Description | Status |
| :--- | :--- | :---: |
| **Product Browsing** | Grid and list views of the urban streetwear catalog | 📋 Planned |
| **Category Navigation** | Filter and partition by collections, drops, and apparel types | 📋 Planned |
| **Search & Filtering** | Multi-attribute search by keywords, price range, size, and availability | 📋 Planned |
| **Sorting & Pagination** | Deterministic sorting (newest drops, price) with offset/cursor pagination | 📋 Planned |
| **Product Detail Pages** | High-resolution image galleries, SKU variant selectors, and size charts | 📋 Planned |
| **User Authentication** | Customer registration, login, profile updates, and JWT session handling | 📋 Planned |
| **Shopping Cart** | Persistent cart management with quantity adjustment and stock validation | 📋 Planned |
| **Customer Wishlist** | Saved items tied to authenticated customer profiles | 📋 Planned |
| **Address Management** | Multiple saved shipping/billing addresses with primary address selection | 📋 Planned |
| **Checkout Pipeline** | Address confirmation, shipping calculation, and order submission | 📋 Planned |
| **Order History** | Real-time order tracking with status updates and itemized receipts | 📋 Planned |
| **Product Reviews** | Verified buyer reviews, numerical ratings, and feedback aggregation | 📋 Planned |

### Admin Dashboard Features

| Capability | Description | Status |
| :--- | :--- | :---: |
| **Admin Authentication** | Role-based authorization (`ADMIN` role guard) and session isolation | 📋 Planned |
| **Product Management** | Full CRUD for catalog items, descriptions, asset URLs, and base pricing | 📋 Planned |
| **Category Management** | Hierarchical taxonomy and streetwear collection management | 📋 Planned |
| **Inventory & Variants** | SKU-level stock tracking across multiple sizes (`S-XXL`) and colorways | 📋 Planned |
| **Order Management** | Order review and status lifecycle (`PENDING` $\rightarrow$ `PAID` $\rightarrow$ `SHIPPED` $\rightarrow$ `DELIVERED`) | 📋 Planned |
| **Customer Management** | Customer directory, order counts, account status, and purchase metrics | 📋 Planned |
| **Discounts & Coupons** | Promotional codes with expiration, usage caps, and percentage/flat discounts | 📋 Planned |
| **Sales Analytics** | Revenue summaries, order volume metrics, and top-selling drop analytics | 📋 Planned |

### Infrastructure and Repository Hygiene

| Capability | Description | Status |
| :--- | :--- | :---: |
| **Client Scaffolding** | Vite + React 19 single-page application setup with React Router 7 | ✅ Implemented |
| **Server Scaffolding** | Express.js 5 + Node.js modular server architecture | ✅ Implemented |
| **ORM & DB Configuration** | Prisma v7 configuration and PostgreSQL connection schema | 🔄 In Progress |
| **Repository Hygiene** | Git audit, strict root `.gitignore`, environment templates, and docs | ✅ Implemented |

---

## Technology Stack

### Current Implementation

```
┌──────────────────────────────────────────────────────────┐
│                   SHADEN ARCHITECTURE                    │
├─────────────────────────┬────────────────────────────────┤
│ Client Layer            │ React 19, Vite 8, Axios        │
│ Routing & Icons         │ React Router 7, Lucide React   │
│ Server Runtime          │ Node.js LTS, Express 5         │
│ Security & Logging      │ Helmet, CORS, Morgan, Dotenv   │
│ Database & ORM          │ PostgreSQL, Prisma v7          │
│ Version Control         │ Git, GitHub                    │
└─────────────────────────┴────────────────────────────────┘
```

### Detailed Component Breakdown

| Layer | Technology | Version | Purpose | Status |
| :--- | :--- | :--- | :--- | :---: |
| **Frontend Runtime** | [React](https://react.dev/) | `^19.3.1` | Declarative component UI library | ✅ Active |
| **Build Tool** | [Vite](https://vite.dev/) | `^8.3.6` | Next-generation frontend bundler & HMR dev server | ✅ Active |
| **Client Routing** | [React Router](https://reactrouter.com/) | `^7.18.5` | Client-side routing and route-level state | ✅ Active |
| **HTTP Client** | [Axios](https://axios-http.com/) | `^1.21.1` | Promise-based asynchronous HTTP client | ✅ Active |
| **UI Icons** | [Lucide React](https://lucide.dev/) | `^1.73.0` | Minimal, uniform SVG iconography | ✅ Active |
| **Backend Runtime** | [Node.js](https://nodejs.org/) | LTS | Cross-platform JavaScript runtime environment | ✅ Active |
| **Backend Framework**| [Express.js](https://expressjs.com/) | `^5.3.0` | Minimalist HTTP web framework and router | ✅ Active |
| **Database** | [PostgreSQL](https://www.postgresql.org/) | `15+` | Relational database engine | 🔄 Scaffolding |
| **ORM / Query Engine**| [Prisma](https://www.prisma.io/) | `^7.10.1` | Next-generation Node.js ORM for schema and types | 🔄 Scaffolding |
| **Security Middleware**| [Helmet](https://helmetjs.github.io/) | `^8.3.0` | Secure HTTP response headers | ✅ Active |
| **CORS Middleware** | [CORS](https://github.com/expressjs/cors) | `^2.8.6` | Cross-Origin Resource Sharing control | ✅ Active |
| **Request Logger** | [Morgan](https://github.com/expressjs/morgan) | `^1.12.1` | HTTP request logging middleware | ✅ Active |
| **Dev Reloading** | [Nodemon](https://nodemon.io/) | `^3.1.14` | Server file watching and auto-restart | ✅ Active |
| **API Testing** | [Postman](https://www.postman.com/) | Latest | API endpoint integration and contract testing | 📋 Planned |
| **Containerization** | [Docker](https://www.docker.com/) | Planned | Reproducible development and deployment environments | 📋 Planned |

---

## System Architecture

SHADEN follows a decoupled **Client-Server Architecture** communicating over a stateless RESTful JSON interface.

```mermaid
flowchart TD
    subgraph ClientLayer["Frontend Client (React 19 + Vite)"]
        UI["Customer Storefront & Admin Views"]
        Router["React Router v7"]
        AxiosClient["Axios HTTP Client"]
        UI --> Router --> AxiosClient
    end

    subgraph APIGateway["Express.js Server Layer (Port 5000)"]
        MW["Security & Parsing Middleware\n(Helmet, CORS, Morgan, JSON)"]
        AuthMW["Auth & RBAC Middleware\n(JWT Verification)"]
        APIRouter["API Router (/api/v1)"]
        Controllers["Controllers\n(Request/Response Handling)"]
        Services["Services\n(Business Logic & Transactions)"]
        
        AxiosClient -->|"HTTP / REST (JSON)"| MW
        MW --> AuthMW
        AuthMW --> APIRouter
        APIRouter --> Controllers
        Controllers --> Services
    end

    subgraph DataLayer["Persistence Layer (PostgreSQL)"]
        PrismaORM["Prisma ORM Client / pg Driver"]
        PostgresDB[("PostgreSQL Database\n(shaden_db)")]
        
        Services --> PrismaORM
        PrismaORM -->|"SQL Queries / Transactions"| PostgresDB
    end
```

### Architectural Principles

1. **Separation of Concerns:** Controllers handle HTTP transport (request unpacking, status code mapping, response serialization). Services encapsulate domain business rules and database mutations.
2. **Stateless Authentication:** User identity is verified via cryptographically signed JSON Web Tokens (`JWT`) passed through standard `Authorization: Bearer <token>` headers.
3. **Database Abstraction:** Queries are executed through Prisma's type-safe client, preventing SQL injection vulnerabilities while ensuring compile-time schema validation.
4. **Resilient Error Propagation:** Unhandled exceptions and validation errors are intercepted by centralized error-handling middleware, guaranteeing uniform client error responses without leaking server stack traces.

---

## Project Directory Structure

The repository is organized as a clean multi-package workspace containing dedicated frontend (`client`) and backend (`server`) applications:

```text
SHADEN/
├── .vscode/                 # IDE workspace configuration (git limits, recommendations)
├── client/                  # Frontend single-page application (React 19 + Vite)
│   ├── public/              # Static public assets (favicons, SVG icon sprites)
│   ├── src/                 # Client source code
│   │   ├── assets/          # Static images (hero graphics, logos)
│   │   ├── App.css          # Application layout styling
│   │   ├── App.jsx          # Root application component
│   │   ├── index.css        # Base styling and resets
│   │   └── main.jsx         # React DOM bootstrap entrypoint
│   ├── .env.example         # Template for client environment variables
│   ├── .gitignore           # Client-specific Git ignore rules
│   ├── eslint.config.js     # Flat ESLint configuration
│   ├── index.html           # HTML5 application shell
│   ├── package-lock.json    # Exact client dependency lockfile
│   ├── package.json         # Client manifest, dependencies, and scripts
│   ├── README.md            # Default Vite template documentation
│   └── vite.config.js       # Vite build configuration and React plugin
├── server/                  # Backend REST API application (Node.js + Express 5)
│   ├── prisma/              # Database schema definitions and migrations
│   │   └── schema.prisma    # PostgreSQL connection and model definitions
│   ├── src/                 # Layered backend source architecture
│   │   ├── config/          # Environment and database connection configurations
│   │   ├── controllers/     # Request handlers and response mapping
│   │   ├── middleware/      # Auth guards, validation, error interceptors
│   │   ├── routes/          # Express route definitions
│   │   ├── services/        # Business logic and database query operations
│   │   ├── utils/           # Shared helper functions and custom error classes
│   │   ├── validators/      # Schema-based request payload validators
│   │   ├── app.js           # Express application setup and middleware pipeline
│   │   └── server.js        # Server listener and database bootstrap entrypoint
│   ├── .env.example         # Template for server environment variables
│   ├── .gitignore           # Server-specific Git ignore rules
│   ├── package-lock.json    # Exact server dependency lockfile
│   ├── package.json         # Server manifest, dependencies, and scripts
│   └── prisma7.config.ts    # Prisma v7 configuration file
├── .gitignore               # Root repository Git ignore rules
└── README.md                # Project documentation and engineering manual
```

---

## Planned Database Schema

The database model is designed around an ACID-compliant relational schema in PostgreSQL, modeled with Prisma ORM:

```mermaid
erDiagram
    USERS ||--o{ ORDERS : places
    USERS ||--o{ ADDRESSES : owns
    USERS ||--o{ REVIEWS : writes
    USERS ||--o{ CART_ITEMS : holds
    USERS ||--o{ WISHLIST_ITEMS : saves
    CATEGORIES ||--o{ PRODUCTS : classifies
    PRODUCTS ||--o{ PRODUCT_VARIANTS : contains
    PRODUCTS ||--o{ REVIEWS : receives
    ORDERS ||--o{ ORDER_ITEMS : contains
    PRODUCT_VARIANTS ||--o{ ORDER_ITEMS : ordered_as
    PRODUCT_VARIANTS ||--o{ CART_ITEMS : selected_in
    PRODUCT_VARIANTS ||--o{ WISHLIST_ITEMS : saved_in

    USERS {
        uuid id PK
        string email UK
        string password_hash
        string first_name
        string last_name
        enum role "CUSTOMER | ADMIN"
        datetime created_at
    }

    ADDRESSES {
        uuid id PK
        uuid user_id FK
        string street
        string city
        string state
        string postal_code
        string country
        boolean is_default
    }

    CATEGORIES {
        uuid id PK
        string name
        string slug UK
        text description
    }

    PRODUCTS {
        uuid id PK
        uuid category_id FK
        string name
        string slug UK
        text description
        decimal base_price
        boolean is_active
        datetime created_at
    }

    PRODUCT_VARIANTS {
        uuid id PK
        uuid product_id FK
        string size "S, M, L, XL, XXL"
        string color
        string sku UK
        int stock_quantity
        decimal price_adjustment
    }

    ORDERS {
        uuid id PK
        uuid user_id FK
        uuid address_id FK
        decimal total_amount
        enum status "PENDING, PAID, PROCESSING, SHIPPED, DELIVERED, CANCELLED"
        datetime created_at
    }

    ORDER_ITEMS {
        uuid id PK
        uuid order_id FK
        uuid variant_id FK
        int quantity
        decimal unit_price
    }
```

---

## Application Workflow

### Customer Journey
1. **Discovery:** Customer accesses storefront $\rightarrow$ browses drops, filters by category/size, or queries specific streetwear apparel.
2. **Evaluation:** Customer inspects product details $\rightarrow$ selects specific variant (color, size) $\rightarrow$ checks dynamic stock availability.
3. **Cart & Authentication:** Customer adds items to cart $\rightarrow$ logs in or registers via JWT auth $\rightarrow$ reviews cart subtotal and discounts.
4. **Checkout:** Selects shipping address $\rightarrow$ reviews order summary $\rightarrow$ submits order.
5. **Fulfillment:** Receives confirmation $\rightarrow$ tracks status in customer account portal.

### Administrative Management
1. **Authentication:** Administrator authenticates using credential pair verified against hashed records with role validation (`ADMIN`).
2. **Catalog Operations:** Admin creates product records, specifies category tags, uploads image metadata, and assigns inventory quantities per SKU variant.
3. **Order Processing:** Admin reviews incoming customer orders, updates order status lifecycle (`PAID` $\rightarrow$ `PROCESSING` $\rightarrow$ `SHIPPED`), and manages inventory adjustments.

---

## Getting Started

### Prerequisites

Ensure you have the following installed on your local development machine:

- **Node.js:** `v20.x` or higher (LTS recommended) — [Download Node.js](https://nodejs.org/)
- **npm:** `v10.x` or higher (packaged with Node.js)
- **PostgreSQL:** `v15.x` or higher — [Download PostgreSQL](https://www.postgresql.org/download/)
- **Git:** `v2.40+` — [Download Git](https://git-scm.com/)

---

### Local Installation

Clone the repository to your local workspace:

```bash
git clone https://github.com/subhasankarsahu/shaden.git
cd shaden
```

#### 1. Setup the Server (Backend)

Navigate to the `server` directory and install dependencies:

```bash
cd server
npm install
```

Copy the environment template and configure your local settings:

```bash
cp .env.example .env
```

*On Windows Command Prompt:*
```cmd
copy .env.example .env
```

#### 2. Setup the Client (Frontend)

In a separate terminal, navigate to the `client` directory and install dependencies:

```bash
cd client
npm install
```

Copy the client environment template:

```bash
cp .env.example .env
```

*On Windows Command Prompt:*
```cmd
copy .env.example .env
```

---

### Environment Variables

Never commit `.env` files to source control. Use the provided `.env.example` templates as guides.

#### Server Environment (`server/.env`)

| Variable | Required | Default / Example | Purpose |
| :--- | :---: | :--- | :--- |
| `PORT` | Optional | `5000` | Port on which the Express HTTP server listens |
| `NODE_ENV` | Optional | `development` | Runtime environment (`development`, `production`, `test`) |
| `DATABASE_URL` | **Required** | `postgresql://postgres:postgres@localhost:5432/shaden_db?schema=public` | PostgreSQL connection string |
| `CLIENT_URL` | **Required** | `http://localhost:5173` | Allowed origin for CORS validation |
| `JWT_SECRET` | **Required** | `your_cryptographically_secure_secret_key` | Secret key used for signing and verifying JSON Web Tokens |
| `JWT_EXPIRES_IN` | Optional | `7d` | Lifetime duration for access tokens |

#### Client Environment (`client/.env`)

| Variable | Required | Default / Example | Purpose |
| :--- | :---: | :--- | :--- |
| `VITE_API_BASE_URL` | **Required** | `http://localhost:5000/api` | Base URL of the backend REST API |

---

### Running the Application

Both applications run independently during local development.

#### Launching the Backend Server

```bash
cd server
npm run dev
```

*The Express API server starts with `nodemon` at `http://localhost:5000`.*

#### Launching the Frontend Client

```bash
cd client
npm run dev
```

*The Vite development server starts with HMR at `http://localhost:5173`.*

---

## API Specification (Planned)

All API endpoints will be versioned under `/api/v1` and communicate using standard JSON payloads.

### Authentication & User Endpoints
- `POST /api/v1/auth/register` — Register a new customer account
- `POST /api/v1/auth/login` — Authenticate and receive JWT access token
- `POST /api/v1/auth/logout` — Invalidate user session
- `GET  /api/v1/users/profile` — Retrieve current authenticated user profile (`Protected`)
- `PUT  /api/v1/users/profile` — Update account profile details (`Protected`)

### Products & Catalog Endpoints
- `GET  /api/v1/products` — List products with search, filtering, and pagination
- `GET  /api/v1/products/:id` — Retrieve product details with associated variants
- `POST /api/v1/products` — Create a new product with variants (`Admin Only`)
- `PUT  /api/v1/products/:id` — Update existing product details (`Admin Only`)
- `DELETE /api/v1/products/:id` — Soft-delete or archive product (`Admin Only`)

### Cart & Orders Endpoints
- `GET  /api/v1/cart` — Fetch user's persistent cart items (`Protected`)
- `POST /api/v1/cart` — Add item variant to cart (`Protected`)
- `PUT  /api/v1/cart/:itemId` — Modify item quantity (`Protected`)
- `DELETE /api/v1/cart/:itemId` — Remove item from cart (`Protected`)
- `POST /api/v1/orders` — Create new order from cart (`Protected`)
- `GET  /api/v1/orders` — List authenticated user's order history (`Protected`)
- `GET  /api/v1/orders/:id` — Retrieve itemized order details (`Protected`)
- `PATCH /api/v1/orders/:id/status` — Transition order fulfillment status (`Admin Only`)

---

## Testing Strategy

Testing will be progressively integrated as features are implemented:

- **API & Integration Testing:** Postman collections and automated test scripts validating HTTP status codes, headers, response schemas, and authentication flows.
- **Unit Testing:** Core business services, discount calculation utilities, and input validation schemas.
- **Database Testing:** Transaction integrity testing against isolated test database instances.
- **Frontend Verification:** ESLint code quality checks (`npm run lint` in `client`) and React component render verification.

---

## Security Architecture

1. **HTTP Security Headers:** Integrated with `helmet` to set secure response headers (`Content-Security-Policy`, `X-Content-Type-Options`, `Strict-Transport-Security`).
2. **Cross-Origin Resource Sharing (CORS):** Explicit whitelist validation restricting API access solely to designated frontend domains (`CLIENT_URL`).
3. **Data Sanitization & Injection Prevention:** Database interactions executed via Prisma parameterization to neutralize SQL injection vectors.
4. **Credential Protection:** Passwords securely hashed using `bcrypt` with adaptive work factors. Sensitive credentials never stored in plaintext or logged.
5. **Repository Cleanliness:** Strict root `.gitignore` configuration preventing accidental leakage of credentials (`.env`), database backups, private keys, or editor files.

---

## Development Roadmap

```mermaid
flowchart LR
    P1["Phase 1<br/><b>Architecture & Git</b><br/>Scaffolding & Hygiene"]
    P2["Phase 2<br/><b>Data & Schemas</b><br/>Prisma Models & Seeds"]
    P3["Phase 3<br/><b>Core API & Auth</b><br/>Express & JWT RBAC"]
    P4["Phase 4<br/><b>Storefront & Cart</b><br/>Catalog & Cart Logic"]
    P5["Phase 5<br/><b>Checkout & Admin</b><br/>Orders & Management"]
    P6["Phase 6<br/><b>UI & Deployment</b><br/>React Integration & Docker"]

    P1 --> P2 --> P3 --> P4 --> P5 --> P6
```

- **Phase 1: Foundations & Architecture** *(Current)*
  - [x] Repository initialization and Git configuration audit
  - [x] Comprehensive root `.gitignore` rules
  - [x] Project environment templates (`.env.example`)
  - [x] Architecture and technical documentation
- **Phase 2: Data Persistence & Schemas**
  - [ ] Finalize Prisma PostgreSQL data models
  - [ ] Execute initial database migrations
  - [ ] Author database seed scripts for initial streetwear catalog
- **Phase 3: Core Backend & Authentication**
  - [ ] Implement Express middleware pipeline (error handling, request logging)
  - [ ] Build user registration, login, and JWT verification services
  - [ ] Implement role-based access control (`CUSTOMER` vs `ADMIN`)
- **Phase 4: Storefront & Cart Services**
  - [ ] Develop catalog browsing, search, and variant filtering endpoints
  - [ ] Implement session/user cart persistence services
- **Phase 5: Checkout & Administrative Control**
  - [ ] Order creation with atomic database transactions
  - [ ] Administrative product, order, and inventory management APIs
- **Phase 6: Frontend Integration & Deployment**
  - [ ] Connect React 19 views to Express API services
  - [ ] Modern streetwear UI/UX layout and design system
  - [ ] Docker containerization and cloud hosting deployment

---

## Contributing Guidelines

To maintain code quality and clean Git history:

1. **Branch Naming Conventions:**
   - Features: `feature/short-description`
   - Bugfixes: `fix/short-description`
   - Documentation: `docs/short-description`
   - Refactoring: `refactor/short-description`
2. **Commit Messages:** Follow [Conventional Commits](https://www.conventionalcommits.org/):
   - `feat: add product variant filtering endpoint`
   - `fix: resolve cart item calculation edge case`
   - `docs: update environment variable instructions`
   - `chore: update dependencies`
3. **Code Quality:**
   - Run linter before committing: `npm run lint`
   - Never commit `.env` or sensitive credentials
   - Keep commits atomic and focused

---

## License

This project is open-source and available under the terms of the [MIT License](LICENSE).

---

## Acknowledgements

- Built with [React](https://react.dev/), [Vite](https://vite.dev/), [Express](https://expressjs.com/), and [Prisma](https://www.prisma.io/).
- Icons powered by [Lucide Icons](https://lucide.dev/).
- Badges generated using [Shields.io](https://shields.io/) and [Skill Icons](https://skillicons.dev/).

---

<div align="center">
  <sub>SHADEN Streetwear &copy; 2026. All rights reserved.</sub>
</div>
