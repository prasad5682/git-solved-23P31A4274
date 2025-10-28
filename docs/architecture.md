# System Architecture

## Overview
DevOps Simulator uses a microservices architecture for production, with development profiles for local testing.

## Components
- **Application**: Node.js + Express (prod port 8080, dev port 3000)
- **Database**: PostgreSQL (prod replication, dev single instance)
- **Monitoring**: Prometheus + Grafana (prod), console logging (dev)

## Deployment
- Production: Rolling updates, zero-downtime, automated rollback.
- Development: Docker Compose, hot reload, fast feedback.

## Security
- Production: strict access control, SSL/TLS.
- Development: relaxed settings for debugging.
