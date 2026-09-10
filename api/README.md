# JobFlow

JobFlow is a study project for backend engineering with Laravel, PHP, PostgreSQL, Docker, Docker Compose, and GitHub Actions.

This repository currently contains only the initial project bootstrap. Job processing features are intentionally out of scope for now.

## Requirements

- Docker
- Docker Compose
- Make

## Local Setup

Copy the example environment file if it does not exist yet:

```bash
cp .env.example .env
```

Start the local environment:

```bash
make up
```

The application will be available at:

```text
http://localhost:8000
```

Run the initial migrations:

```bash
make migrate
```

Stop the local environment:

```bash
make down
```

## Common Commands

Install PHP dependencies:

```bash
make install
```

Run tests:

```bash
make test
```

Check formatting:

```bash
make lint
```

Apply formatting:

```bash
make format
```

Open a shell inside the application container:

```bash
make shell
```

## Out of Scope

The following parts are intentionally not implemented yet:

- job tables
- job-related models
- queue workers
- processing commands
- handlers
- retries
- scheduling
- Redis
- job APIs
- business rules
