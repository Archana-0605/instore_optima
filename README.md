# InStore Optima

A full-stack retail management system developed as a team project for managing
inventory, procurement, orders, and payments.

## Tech Stack

- React 19
- ASP.NET Core (.NET 8)
- Entity Framework Core
- SQL Server
- JWT Authentication
- Docker

## Features

- Inventory management
- Stock automation
- Procurement management
- Order management
- Payment management
- Role-based access control
- JWT authentication
- Two-factor authentication
- Audit logging
- Automated testing

## My Contribution

This project was developed collaboratively as a team project. My primary contributions
focused on the User Management and Audit Logging modules.

### User Management
- Developed the user management functionality for viewing and searching users by ID,
  name, email, and role.
- Implemented role-based access for user management, with Admin/Manager access to
  the user module and Admin-only user deactivation.
- Implemented soft deactivation by changing a user's role to `Inactive`, preserving
  existing orders and audit history.
- Integrated account-deactivation email notification and the frontend undo workflow.

### Audit Logging
- Developed the Audit Logs module for viewing and managing application change history.
- Implemented audit log retrieval with filtering and search by action, audit ID,
  entity type/ID, user, and description.
- Implemented display of `OldValues` and `NewValues` JSON to inspect changes made
  to application entities.
- Implemented CSV export of the currently filtered audit log records.
- Worked with the EF Core audit interceptor to capture authenticated entity changes
  including the actor, action, entity, and before/after values.

## Project Structure

- `src/` – Application source code
- `database/` – Database scripts and related files
- `PROJECT_DOCUMENTATION.md` – Project documentation

## Team Project

Developed as a collaborative academic/team project.
