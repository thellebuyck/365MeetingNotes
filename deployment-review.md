# Deployment

These are the notes that are centered around deployments

## Containers

1. using Docker and compose for production - written by Nunley.
1. seneca microservices (flight check, caldera, KISS Cut) - Jamie Fellwock
    1. microservices (Product) - Deployed using Docker Compose
    2. 2 containers on 4 services. use api gateway
    1. Don't use the gateway for kiss cut

## Web Applications

1. Admin Site/Signs 365 Site
    1. V3_Complete - The project contains source code for both sites
        1. v3_complete repo is primarily the frontend/backend/api code (this is always pointed at latest of master before deploy).
    1. using the GitLab CI/CD pipelines to deploy the applications
    2. We want to split the production deployment for frontend/backend and api code.
        1. Somewhat for the development.
1. Maintenance
    1. Static maintenance page so to that we can perform maintenance without outside traffic hitting the sites
1. Imaging
    1. Supervisor control (Linux managed process) to make sure the processes are running.
    1. Memory leaks that we are aware of?

## .NET Projects

1. all click-once deploy
1. need to work on encrypting the connection strings

## Database Changes

1. Eric/Drews handle propagating changes to the database
    1. Most team members have access
        1. Employees - Read/Write
        1. Contractors - Read-Only
1. No strong process for deployment
    1. Code reviews - need to apply a consistent patterns
1. 