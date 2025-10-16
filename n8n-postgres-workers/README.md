# n8n with PostgreSQL and Workers

n8n setup with PostgreSQL database and worker nodes for distributed processing.

## Quick Start

```bash
docker-compose up -d
```

## Components

- **n8n**: Main application (port 5678)
- **PostgreSQL**: Database
- **Workers**: Background job processors
- **Redis**: Queue management

## Scaling

To add more workers:

```bash
docker-compose up -d --scale n8n-worker=3
```
