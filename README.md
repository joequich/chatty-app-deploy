# Chat App

Instructions to run the entire application locally

## Prerequisites

- Node.js v22.13.1 or higher
- pnpm v10.3.0 or higher
- Docker and Docker Compose

## Clone the repositories

Open a terminal and run:

```bash
git clone https://github.com/joequich/chatty-backend.git backend
git clone https://github.com/joequich/chatty-frontend.git frontend
```

Make sure that both repositories are in the same root folder.

## Database environment variables

Create or edit the `docker.env` to set up the initial PostgreSQL database.

Example `docker.env`:

```env
 POSTGRES_PASSWORD=yourdbpassword
 POSTGRES_USER=admin
 POSTGRES_DB=yourdbname
```

## Lift the services

From the root of the project, run:

```bash
docker-compose up
```

This will start the backend, frontend and the PostgresSQL database.

## Notes

- Adjust ports and environment variables according of repository configuration if necessary.
