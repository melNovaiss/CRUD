# Simple CRUD
This repository contains a simple CRUD project built using Java, Java Spring, Flyway Migrations, PostgresSQL as the database, and Spring Security and JWT for authentication control.
The aim of this repository is to practice and share how you can build all CRUD Methods using Java Spring.

## Table of Contents

- [Installation](#installation)
- [Authentication](#authentication)
- [API Endpoints](#api-endpoints)
- [Database](#database)

## Installation

1. Clone the repository:

```bash
$ git clone https://github.com/melNovaiss/crud.git
```

2. Install dependencies with Maven

## Usage

1. Start the application with Maven
2. The API will be accessible at http://localhost:8080

## Authentication
The API uses Spring Security for authentication control. The following roles are available:
```markdown
USER -> Standard user role for logged-in users.
ADMIN -> Admin role for managing partners (registering new partners).
```
To access protected endpoints as an ADMIN user, provide the appropriate authentication credentials in the request header.

## API Endpoints
The API provides the following endpoints:

```markdown
GET /product - Retrieve a list of all data.

POST /product - Register a new data.

PUT /product - Alter data.

DELETE /product/{id} - Inactivate data.

POST /auth/login - Login into the App

POST /auth/register - Register a new user into the App
```

## Database
The project uses PostgresSQL as the database. The necessary database migrations are managed using Flyway.

To install PostgresSQL locally you can [click here](https://www.postgresql.org/download/).
