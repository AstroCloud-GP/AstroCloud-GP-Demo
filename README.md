# AstroCloud GP Documentation

The purpose of this documentation is to provide insight into the AstroCloud GP project, including its features, demos, and architecture, without exposing the actual codebase as it is closed source, in hopes of growing into a commercial product in the future.

## Overview

Welcome to Egypt’s First Managed Cloud Hosting Platform!

AstroCloud is a Platform-as-a-Service (PaaS) developed as a graduation project aimed at empowering developers, startups, and businesses in Egypt with a fully managed cloud hosting solution.

AstroCloud simplifies application deployment and infrastructure management by supporting static and dynamic site hosting through GitHub integration or ZIP file uploads. It features an intuitive dashboard for managing deployments, along with continuous deployment, automated builds, and real-time log streaming.


## Demos

**Main Demo**

A comprehensive demonstration of the project, in which we deploy a full-stack registration system consisting of a backend and 2 frontends.

[![Main-demo](https://img.youtube.com/vi/aHG26cFSSnQ/0.jpg)](https://www.youtube.com/watch?v=aHG26cFSSnQ)

[![AstroCloud Main Demo](https://markdown-videos-api.jorgenkh.no/url?url=https%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3DaHG26cFSSnQ)](https://www.youtube.com/watch?v=aHG26cFSSnQ)

**Extra Features Demo**

Showcasing additional features such as CI/CD, instant rollbacks, and more.

[![extra-features-demo](https://img.youtube.com/vi/0wn3IJjWljs/0.jpg)](https://www.youtube.com/watch?v=0wn3IJjWljs)

<iframe width="560" height="315" src="https://www.youtube.com/embed/0wn3IJjWljs?si=0Bmxb53KNH8umihR" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

**Landing and Documentation Page Demo**

A demonstration of the landing and documentation page, which serves as the first point of contact for users, providing an overview of the platform, its features, and user documentation.

[![landing-page-demo](https://img.youtube.com/vi/KC1RmH3aVEc/0.jpg)](https://www.youtube.com/watch?v=KC1RmH3aVEc)

**Admin Dashboard Demo**

A demonstration of the admin dashboard, which provides administrative functionality such as user and project management, user plans, and system statistics, and more.

[![admin-dashboard-demo](https://img.youtube.com/vi/rklRAFE2zVg/0.jpg)](https://www.youtube.com/watch?v=rklRAFE2zVg)

## Features

### General Deployment Features:
- GitHub Integration.
- SSL certificates for deployed applications.
- CI/CD pipelines for automated deployments from GitHub repositories on updates, for both static and dynamic applications.
- Live build logs streaming during deployments, using WebSockets and Kafka.
- Edit and rebuild applications directly from the dashboard.
- View previous builds and their logs and status.

### Static Hosting (Frontend Websites):
- Deploying GitHub repositories.
- Building frameworks like Angular, React, Vue, and Svelte.
- Supports ZIP file uploads for static sites, using pre-signed URLs for uploads.

### Dynamic Hosting (Backend Applications):
- Deploying Node.js applications.
- Deploying from GitHub repositories or ZIP file uploads.
- Health checks and automatic restarts for applications.
- Auto-scaling capabilities based on traffic.
- Rollback support for previous versions.
- Kernel-level isolation for security and performance with MicroVMs.
- Runtime Logs accessible through the dashboard for debugging and monitoring.

### Side Features:
- Login with GitHub and refresh tokens for secure access.
- Monorepository setup for sharing code between the backend and the various frontends.
- User Plans authorization system for managing user access and features.

### Automation and DevOps:
- Automated production deployment pipeline for our system, to deploy the whole system with a single click.
- CI and quality assurance checks for all pull requests.

## Detailed Documentation

For a deeper dive into the project, please refer to the following documents:

- [**Project Architecture**](./project-architecture.md)
- [**Project Management**](./project-management.md)


