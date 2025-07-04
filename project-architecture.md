## 🧩 Sub-Projects Overview
The project is organized as a **monorepo**, containing multiple related services and shared packages within a single repository. This structure enables streamlined development, unified dependency management, and seamless code sharing across the backend, frontend, and platform components.

### 🖥 [Backend](./apps/backend/README.md)

- Provides a REST API using Express
- Real-time communication via WebSockets
- Integrates with PostgreSQL, Redis, Kafka, GitHub App, and Azure
- Handles authentication and background job queues

### ⚙️ [Platform](./apps/platform/README.md)

- Interfaces with containers and cloud infrastructure using:
  - Dockerode
  - Kubernetes Client for Node.js
  - Azure SDK
- Executes privileged tasks and coordinates service orchestration
- Pushes results to processing queues

### 🌐 [Frontend](./apps/frontend/README.md)

- Built with React and TailwindCSS
- Sub-projects:
  - `admin-page/`: Admin interface for managing users and system state
  - `landing-page/`: Public-facing landing site
  - `user-dashboard/`: Main user experience for interacting with the system
  
### ♻️ [Shared](./packages/shared/README.md)

- Type definitions shared across all sub-projects
- Common constants, utilities, and services
- Promotes type safety and code reusability


## 📁 Folder Structure

```
AstroCloud/
├── apps/           # Main sub-projects:
│  ├── backend/      # API, WebSocket, database, GitHub App
│  ├── frontend/     # UI: landing, dashboard, admin
│  └── platform/     # Dockerode SDK, Kubernetes, Azure integration
├── config/         # Docker services configurations
│  ├── gateway/      # API Gateway configuration
│  ├── smee/         # Webhook delivery proxy
│  └── webserver/    # Static webserver setup
├── infrastructure/ # Infrastructure as Code (IaC) and automation
│  ├── ansible/      # System configuration & provisioning
│  ├── scripts/      # Utility scripts for deployment/dev
│  └── terraform/    # Cloud IaC definitions
├── packages/       # Shared modules across apps
│  └── shared/       # Shared types, constants, and logic
├── docker-compose-prod.yml # Production docker compose
├── docker-compose.yml      # Development docker compose with file watching.
└── Dockerfile              # Root Dockerfile for multi-service builds
```

