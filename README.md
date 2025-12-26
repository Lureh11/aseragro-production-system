# aseragro-production-system
Internal production system for managing machines, technical drawings (PDFs) and role-based access control.

This project is intentionally built without Backend-as-a-Service solutions
to consolidate fullstack and backend fundamentals.

---

## Project Purpose

ASERAGRO Production System is designed to centralize and organize the production
process of industrial machines by:

- Managing machines and their production metadata
- Storing and versioning technical drawings (PDF)
- Enforcing strict role-based access control
- Providing traceability and auditability across the production lifecycle

The system targets small internal teams (15–50 users) and prioritizes clarity,
security, and maintainability over unnecessary complexity.

---

## User Roles

- **SuperAdmin**
  - User and role management
  - System configuration

- **Designer**
  - Create, edit and delete machines
  - Upload, update and remove technical drawings (PDF)
  - Manage production metadata

- **Production**
  - View machines and drawings
  - Download and consult PDFs
  - Add production notes and update machine status

Permissions are strictly enforced server-side.

---

## Learning & Engineering Goals

This project is used as a hands-on exercise to consolidate:

- REST API design with Node.js and TypeScript
- Relational data modeling with PostgreSQL
- JWT authentication and role-based access control (RBAC)
- File storage and versioning strategies
- Audit logging and traceability
- Dockerized development environments
- CI/CD pipelines using GitHub Actions
- Clean architecture and maintainable code structure

All architectural and technical decisions are documented as part of the project.

---

## Planned Architecture

**Backend**
- Node.js + TypeScript
- Express
- PostgreSQL
- ORM: Prisma
- JWT authentication
- RBAC middleware

**Storage**
- S3-compatible object storage (AWS S3 / MinIO)
- PDF versioning support

**Frontend (planned)**
- React (web)
- Role-based UI rendering
- PDF preview and download support

**DevOps**
- Docker & docker-compose
- GitHub Actions for CI
- Environment-based configuration
