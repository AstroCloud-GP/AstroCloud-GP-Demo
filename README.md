# AstroCloud GP Documentation

The purpose of this documentation is to provide insight into the AstroCloud GP project, including its features, demos, and architecture, without exposing the actual codebase as it is closed source, in hopes of growing into a commercial product in the future.

## Overview

...

## Demos

1- Full Demo

2- Landing and Documentation Page Demo

3- Admin Dashboard Demo

## Architecture

![architecture](assets/image.png)

### Main Components

- **User Dashboard**: ...
- **Admin Dashboard**: ...
- **Landing and Documentation Page**: ...
- **Backend**: ...
- **Platform**: ...

### Other Components

- **Database**: ...
- **Redis**: ...
- **Kafka**: ...
- **Nginx**: ...
- **Azure Blob Storage**: ...
- **GitHub**: ...
- **Kubernetes**: ...
- **Container Image Registry**: ...

## Features

- General Deployment Features:
    - GitHub Integration.
    - SSL certificates for deployed applications.
    - CI/CD pipelines for automated deployments from GitHub repositories on updates, for both static and dynamic applications.
    - Live build logs streaming during deployments, using WebSockets and Kafka.
    - Edit and rebuild applications directly from the dashboard.
    - View previous builds and their logs and status.

- Static Hosting (Frontend Websites):
    - Deploying GitHub repositories.
    - Building frameworks like Angular, React, Vue, and Svelte.
    - Supports ZIP file uploads for static sites, using pre-signed URLs for uploads.

- Dynamic Hosting (Backend Applications):
    - Deploying Node.js applications.
    - Deploying from GitHub repositories or ZIP file uploads.
    - Health checks and automatic restarts for applications.
    - Auto-scaling capabilities based on traffic.
    - Rollback support for previous versions.
    - Kernel-level isolation for security and performance with MicroVMs.

- Side Features:
    - Login with GitHub and refresh tokens for secure access.
    - Monorepository setup for sharing code between the backend and the various frontends.
    - User Plans authorization system for managing user access and features.
    - Real-time notifications for deployment status and errors.
    - Custom domain support with DNS management.

- Automation and DevOps:
    - Automated production deployment pipeline for our system, to deploy the whole system with a single click.
    - CI and quality assurance checks for all pull requests.

## Sections

- [**Project Management**](project-management.md)


## Contributors

- [Ahmed Atwa](https://github.com/nightknighto)

